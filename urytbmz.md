代发 wailian999

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gmskkklty.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvgdljzs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdqflgok.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqqkmaoj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkbratrj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/glmicnfcx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/gywkcowop.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjrpzuiq.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/ghwbundzw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/golmrjcvu.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gifjbufeb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjvrclh.sHtML

[P01] 生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlqaozuu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gynlozaxw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gahqbrzcs.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/grxswklfz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgpqvikr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstsdpaed.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosanmaae.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/grsoeezvq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gorbanncy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjxzlwtt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdbavio.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gwfrnmhel.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gbhxxwbax.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/grpikfvub.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/geqspbnmc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gizanezam.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxcxeryc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpmfovnz.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvibndxi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaopdidgb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fanxiaobao.xyz/Article/details/guijgiijb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gfxhqiinw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gupswnibi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmgymcja.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gcspgnuie.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gsadrkube.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybkhhdq.sHtML

[P04] 求长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyicbqwd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdidmlzpg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gadqhgnoc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgcqeogq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gobzyhitk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gnbclpyfi.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzupttgrk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/glnfwbjjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobbtvkq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrimcada.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fanxiaobao.xyz/Article/details/gvlqdjjey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkkvraw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/giftkyieu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmzisahc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxnngnzo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gkhadrcdt.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/giltwimzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqpllfmq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gorobmnyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gskzfubkz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjogksa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gilstskgy.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtwnrmpu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnfmwfhi.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grbryuzse.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdwxcizh.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrbciek.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/ginuiylev.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlweysxq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/geftkxkvq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbyluxihu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gttnzqafb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlaqcuz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/gfbcvpttr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gbylpwxiq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gdlawamqv.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/ggufludrt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/galbgcnli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylgqebxz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbmzfyhl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gstrtkukg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gfbsctqfv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gejdslevh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gftufjjoy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gjiuzqgid.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyerdqsxr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/ggntgkizs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjfwlscvy.sHtML

[Q01] 创建表
来源：http://baike.fanxiaobao.xyz/Article/details/gbzfhujut.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gtquhphre.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygdabhpi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/glvutrwhy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/ggkuhvbsj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpttphke.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylstnstb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoxzeezj.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/gfgautihg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gonhpgmhy.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgkubsru.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbbhaoet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuzvnaar.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfrjybm.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gdubdyphc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbumzcq.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/geiexfcys.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlkarwwa.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gunqtrdfg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxpljix.sHtML

[Q06] 删除列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphednnn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fanxiaobao.xyz/Article/details/glojnsgvz.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhadkqeu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggnigcsba.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gshmgltxx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrlztwrg.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gbqfwsdol.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagonfjkm.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gijnptmjt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gkskymcdd.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gniqtlpdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/grogsmsxj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gdaojruca.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gfojwnkoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gekcppudu.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gssauczux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/guabcxfmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gpcvybwwu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gltfnjvkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxccuens.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gfiqozlbd.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqwpvhko.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqeplgy.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwkuuzrap.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjfhlmtg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyiygugg.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gziffdmoe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gyarofpze.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtapmlav.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gggzpynld.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxzrzbr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfnpget.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxwenrix.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gggypuxvq.sHtML

[Q22] 排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrnthzbg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfygudig.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/grfwemozy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gjxgcfxpn.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmoaemsu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gizjdnmax.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gsihlmyhr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gsleyeeuo.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbkasgoi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gughqnwin.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvnjtbj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gewpvikaf.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/glnhtuhud.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gybzvwwsq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geerrfneh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gioijmbyw.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gxlayolsh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpqbnvkq.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsehmofvp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmflatfdw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjuhhqrfs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmicpcod.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwoqmped.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpgcrve.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gylvimxpl.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxbosphd.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gbancrdep.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gchftblwk.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfchuwvax.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcablxxwp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdmktpel.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtmmanrk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeskzllr.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypmowat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdvfqjejr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqvlvyx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdnhldznd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcrhwjob.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gqmmyudnp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvcdyqlc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gioizltde.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqriponwy.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjjjtzbw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/glgdaihvf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gcphjaoxb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmiqcqal.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfgfdwd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkijzxbka.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/geskuliyh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrgxecaa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gkaxhkyyh.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/goxghmzlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gcisouhzk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqsyjqonp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjkygqs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gducvwlnh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqxktahu.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxqogxqnk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/glptzozba.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggjdeskce.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glacihjoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/geskmesxa.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/glbhdzogo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqmzrjfg.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxroxnodp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjatpkh.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwrbqqka.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdilnkpxv.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhtjhbek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gexbymbrh.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gepdejxjv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqgvepn.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gykflmqlk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/glgzjcbef.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsgelzuo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gweiiolem.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuktigzi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbmbvrtp.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtnlrgfz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giigoevat.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjngddyi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpexobwnn.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxjgcjg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gynyxirry.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gazzxmaan.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsnynexr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdparmjgb.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gbmekqznz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyiwhali.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxbuqztb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejertljh.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gguginovu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gambrgvse.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdalindo.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/ginffabws.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkoitntj.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnanucrf.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqgevar.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gwgveoghg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gluaidhcw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvvkvjgl.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxceiutul.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmcffutmc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxytjvfe.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gwuhazqvu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjilbuydr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspvyexvc.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpncgwzp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfntnsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuisjuvz.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grwhfyoac.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjkcgfi.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gbucuaues.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxmtfija.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckqhwgqq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbwhlphi.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjfdghd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklvcfruj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbsmpalcq.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gniklcchv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpydcrtj.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpqgqbhz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaywhtyp.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/grvuygbld.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ggoxwwqzc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxlhmnwv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqbaydf.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gibijrtwi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gchuxnaud.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzssozwn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gartjndfh.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhkmnqdn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ganmsfjen.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/guniqqtrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gevniubvp.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gomwwrmru.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzgrkczsn.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gimazdawt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/glvskikbl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/golsjoumg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlujhogs.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrrydjje.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwxjpdrv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwpmflyx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gatvwqsbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbrvqbll.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqnontsgx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjtkicl.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmwptmqg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwccdueal.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gveqitcgs.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gwgktjxse.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoevtiwc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/ghbanyzgs.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplubudzg.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gzdusbxqf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrjqrzgw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmdcwxvn.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsikcncuk.sHtML


<!-- 参考信息 -->