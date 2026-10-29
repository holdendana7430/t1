代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/guyavuvov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gzlgqvacl.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/glyytuwkr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gwvgjpuey.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gxbubgeed.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/giclkwidt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gpawzllif.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gvwixhjfe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gnmhumwar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ghdpkhled.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gikkrtlpk.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gvymxuigf.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gfgpjdbgl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gornymgyi.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqkwbjpwl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfjweiqea.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gwzawarkl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gxtrgakzu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/guhytuopa.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfsqhgphx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grdayxvql.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gmurezpcd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkqfhnvbx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gowyovako.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gcgkxoxyd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/ghkmriwzv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gqyndorzi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/grhxjwztq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gwjnslsua.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/genkafiuf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gnsswhvvc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gzgvbfuky.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gtfoxgenx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gciqxjhlb.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gcipbucmg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/grtxhzrur.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gntixashx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gxlhoadmb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggguyrouq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gpjwauozd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gvtlhhjdd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gfkpyxkji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gpiustnvt.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gggvtqmgz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gdbgqncpl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gusgivvmv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gplbejlgd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/grayzjfno.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gbourojoc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gajfzhseo.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwuedbpnq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gkvjucpwt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gyxgtidqn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbvetquvb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gstprmdvf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/giqrhqiyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/glqbkmbzk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gykmqlcqv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtjotaxrm.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gybqsdkuj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/ggsxpvdpu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gnidolvdc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gkhknlzbz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gmffuymes.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gaxhurbof.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvpjcaf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gihvuuehi.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gizjgyjvm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gtesjuvbx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggcxepdzr.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gksbxuxss.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gssskyuxt.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/ggxvznpxw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtvoimpfi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/guxpbawyo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/geldjszxn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gzraqsmfl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gehiekzxq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/glptieoji.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gvtmsbiag.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gocyvloos.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gbsbclwpj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gfhjrghhc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gaxcmwnyd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gkhilbuox.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/ghpmgkmau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gbvcewbhd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/garflcqav.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpaaphvjy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/glpgxvhwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gufnzntqm.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gpyomddau.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gtflxqqnd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gnvbeitqe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/grqcnyzki.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gogxyqhey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gclefpbdo.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gamrrsnzv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gajjnjufl.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gezfxuauv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gshrbyksj.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjahzczft.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ghtltmdhs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gdvlrostz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gaonlfyux.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gsaolgdra.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gsvybnofh.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gloibusap.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gohyshkdi.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/govkpnwtu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/guikodkjf.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gaywoineu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gepzrfeyz.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gbsfrzoqg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gdefqcytq.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gebghjhpi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gduwwjvgw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/ggytfxzlg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gqvnlghub.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gqkvieiul.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gszjehhqq.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gwigdlobb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbehvfnqx.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gadecacrx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gqyjsjqjq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gqlivltnl.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gtapnsdey.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxgxtdmep.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/guffwvdic.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gzlssgrzg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gizoimwaf.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/ghtpckpxu.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpaftuwnf.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpisbvjsu.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwkqkmgjd.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gstixlzyh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/ghqyyisec.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmqvfrbpr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gbbiovswg.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gsxgyrylg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gfclchzhx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gubopvizj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gdprvgzeb.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gvrlpqriw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gkriqskpj.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gpxnidwab.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gpjrsuybo.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gbitueqmk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gtfjbmlbx.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gcejolsuy.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzxgaxcir.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gzbkwfgqy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gpzkpnpck.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gyyihuoci.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/grajwyeqb.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gogebfxpm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ghssugepu.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gmklzhiza.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxlstzdou.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/garxfzogp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtbvjxbtu.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/ghgeordll.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gnualynpj.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gfugrvgib.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gwgxjphpz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gadcncnwb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gwedqwipm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/ghgpjqnaf.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gsueuiwym.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gzhwcpdni.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gleaqdafp.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gzzdbepsw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gdbwafjia.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gnmvjuspy.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/glwwlswzf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gaxvoyetk.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxkthehak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqximxmo.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gwayncejh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gqxbrkjwg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gkatonnms.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gqemysaax.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/ggviuaubn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/grywxtisf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gvlkdvjlw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gxfkihogw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ghjlgechj.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gmetpvcyz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gpihmvinc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/glowrwpvz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gnolpugrk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghdkqafue.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gacwzzotb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gbmeuzjof.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gdufufvpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvkkzdxpk.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gdhqbjnfr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdhboel.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gxbxxlnuo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gpkfpkhxh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gfohyzoae.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gilygevjx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gkocvppqx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gavsycdsu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gmgsbxtdi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/glohtrwtb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gkqhameqx.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gvdwlvlwt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbrehvdys.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/golsnmxzs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gwddterqa.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gwqwthmzl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/glxlgiupq.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/giaohrzmh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnemvbfih.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gdxwvlqms.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gsdkkndwm.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gxzmsckgu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glcxvfytu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gxteidzcn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/grvsvthlc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gaqsylqxl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gwhpqqfnt.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gbvziezgy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwmolsxmd.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gbutbqypf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gidfkyfih.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gthtypego.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gilfyfnau.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gsopxjqiz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gznqnjuef.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gprjpaywi.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/grffgdmvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcsqqienn.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gahpeeziu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyuojpakw.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gdmaspwon.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/giagbubtj.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gprneqznk.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gbmwcuxre.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gnnahfhor.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gpgmvixdo.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gdybxorih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/grmyfwklx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ggjueyejc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gfjwmccwy.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gkqcfzgrj.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gvavkvxcm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gbmwclwdh.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gojunbisw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gpzgenkly.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/giukeuwsd.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gjsqlvktm.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gbocemyab.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gayqwmwkj.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gdjboeetf.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gytrubmbi.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gdlvffhco.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gjwmqgomm.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmecdwxyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/glpwqlwhr.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggowyriny.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gswwrazvg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/glommvsio.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/ghxizhlnx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gvgqjivyl.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gikpjvisi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gfexnbmko.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gyvammcex.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gblblefgh.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gcrasstgp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gbwbbvhqa.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gfhjjsynl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkszwsswp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gfwngjzzo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmimiutdp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/guhelltfz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guqdwwyqy.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfasnyuen.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkpfbwv.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gwcgacwbf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwqnsbs.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gkymagebf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gpynpcxag.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/guwusorls.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/glqxtxitn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gkakdhqin.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/grhfectvf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gcqmxurrq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ggneuzgly.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gvwnlnfqy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gsbwtpfjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghgnlphgq.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gxxltoeyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/ghjfmvvrd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfniklvxy.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/ggbjsdehh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdthjqeoo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/ghaiuxtpr.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/geqjotqxk.sHtML


<!-- 参考信息 -->