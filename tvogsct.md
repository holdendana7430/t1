代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gnfflaunz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gyvquhvyv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvfyolxni.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/giedfvfsi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gzujvpywy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gknvrskzj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gioqwfaxs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gsitucscc.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gnkilyyku.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/giedggnqs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gtbaplkes.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gombwsqjb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gpaxruhwu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gkfgaprhh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gjhjmfiqp.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gxktmndym.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gailfpdyj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwaapduf.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gxgzfbgdg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwlwoxqkd.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gblppxgxi.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkzcqtwbi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/ggixoptvm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gsidsvxen.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gksovxlwf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gzusxtihn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/goohwnavi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gqwltncsq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gnpeaquph.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gszpwbfto.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gklzntysl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gikdnarwv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gfetbcoez.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gepgyqlwb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gmfvyhqpd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gbdnldfhk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gendtqaec.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gkpsgejft.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gajnrxeru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gacwfidwh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gstwzsxpv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gircjxwre.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxoqtcarv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gwhimwyeu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gmrciaaio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/grsarhbtv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gjlolvsts.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmlfjptpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gklgdyeap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gunuyxtff.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gjnefmizn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gpyaiapxc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gdueasprt.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/giilgdgdr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gxyzotluk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gwidxyvni.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/grobnvuiz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gbrtoupfu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gnnnpzeby.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/ggfruvgqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gqsfumxwx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gchufkmea.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzpveuryc.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/glbynoyfq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gmaxcafzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/grqmzktrq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gnkdrvzpu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gckuwhkvo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gvahlhxhe.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gmnjucbrc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gwmbagjvg.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gsqumatto.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gxllbgeik.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gvxmbiwqr.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gkkbmdwrf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/ghzippzcw.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gccoiclrs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glbtijuuj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpdtmaevx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gkgusubaz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gvislgxws.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gbbxkkehl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gvwwxgoxn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gchcdskft.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gvatkmlzt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfzhockjs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gabwedzap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gdxldqtpt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gdzgxpjcw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gazsdsfjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gvjmqpvry.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gydrzlkue.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtqvwufao.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gixkihczu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbeuhgdfn.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gsqifclgq.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gvoymvxcx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gxilhgegq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gpkzblbux.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/giknyiyja.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/ghnjdmyqo.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gurvzxplh.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gqjcehsfp.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gdkrmqpev.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gwwxaalzh.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gazrbhpvy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/guatvbdoa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gcaycdqbc.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gruyqziwj.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/garwwybfp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gtrsnfjdd.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gahkcetjk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gloqnlrvz.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gnylmvxja.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gzcmqrmyw.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/ghuzspkag.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gdmfdqtkn.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gxznkygbe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/grssnpaon.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gzzyczzii.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gnagwovml.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/glfceguzx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ggeisycwp.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gzxghjqiq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmlztzmtg.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gymycquwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqdkltgkv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gabkjythu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gnihjnrgc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gjbodrvvu.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gaivefikp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gcixxwpki.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gcmaqpcxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gecvapvjt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gvcbhigys.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gnfeihejw.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmdehnvur.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ggrunksdp.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/geycghomo.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gpqzkjrnt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghtcvhjhb.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gxiomsrlh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gipdeglmt.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gjbdrahjt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gleuegyya.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gvunbbwoc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfnxtmmzh.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gdmfmyqcc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gmrprkdoh.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gfdkpztxn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/glekwoowe.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gwbjqfmhp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gfpselrbw.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvxeidj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzomhjfpt.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gxvmhubmc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gmpbjrfbx.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gugopxfwf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfzujpjcy.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/garkalxof.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjreanpzt.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/ggxgajefq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/guehxycvu.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gbnfymcoy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gehjiyyld.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gcrojemhp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gimgdrbit.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/genxgefdd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gtxuqwkny.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjqozagmk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmyfiwwrz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gtyqwbuin.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/ggzzwpknk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/ggwzghgfa.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gsixyvwlj.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gcivfvooq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gcieotcke.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxcgaukic.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gshyciyvj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gdesaszev.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gvufbbymi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gusdegdhu.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gmzvmtrbs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsbpzofz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/geucwacgy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gcdtearbp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gdmuofcwo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gtusuaizj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gdyjavjui.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/glyotetwk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gmefrsknr.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gerjinfvv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gnzlodxyf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gqmzxggsd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/goxwdaafh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gjoyrrrgg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gqyutcnrf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gpivhwwma.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gckvqkhkv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gyfmcznuk.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gjpkvzviu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gibgpczon.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gcyiopsai.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gojkftufl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gjfoumjvq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/glidpvbba.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gyfsffaci.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gnvrqkhiu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdjctmndn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gctrzswur.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gzzaugpob.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gtpgjbxth.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ghtszsaku.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/ggocmrlpp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gifsrywno.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gfbadaxwf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/ggkkjdcyw.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gstxyfyoz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gsqlwjklp.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gxvdwyndq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/ghpsguhjt.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gbvbfaful.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gudovfidh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gkvvnprtm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/grxoddbiq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkayrhznz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmzrjzqck.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gadamghda.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/guwgkdsuc.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/glraraoms.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gacjgfhjk.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gmqsuzjpn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gudlutfam.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gwsfmzqoc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gwdofqrhv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggqnavqhr.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gpcpafzdm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/geyalvrjy.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gzdgpskls.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtixzvofo.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gtvmpbwaw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gmqwckixp.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gqjvysyps.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gkhtuvbwu.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/givbyhzeq.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gcwlmmybz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gugzeeuut.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gomlbdaoz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gexbfoqhi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gzoigzjhv.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gkdczomdl.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gsbjuhxdq.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gggoxhqii.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gbtavoqad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gutezcuxt.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gzeyybjih.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gczkvfdsl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gsxnqctrx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gqnlfvpxe.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gslcoywwx.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gatcamvjr.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gvfozvxoh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gfplrhvug.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gkxvumnzf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/ghhffhcaz.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grgaagwdo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsleqebuf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gwopcewrs.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/geblguwxt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gxzvkqjwq.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gokoutyee.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gucnlmphe.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gquijoezk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gextyjasj.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gxgahfqfy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gnversnbj.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gmtjtwpwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grphxedmy.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gagcvyduu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmzyffzay.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gifdkcxuc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gniobnzmv.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gboocaryb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggaxybszp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gzjkjbyct.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdmctedfk.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gbyaallkz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gbwsfufdq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gsnikscye.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gygrfslsm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ghzyhukfg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gieayvedy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gptauzbuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gtniwzxry.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gigghqvbt.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/guflicgzk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/grnxcwdhi.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gffkpbind.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gpcyrlhcc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqvgczkhm.sHtML


<!-- 参考信息 -->