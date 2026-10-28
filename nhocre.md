代发 wailian999

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtpesscxil.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtjtdskwao.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtaykdglke.html

JS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtvduxhtbg.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtmyriazhy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtxqatdqkr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.havefunace.top/gtfutnfepv.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtoqlquycy.html

C#:   Parallel.For
来源：http://hz.hnxiangtu.top/gtutyqcgqk.html

================================================================================
来源：http://hz.hammf.cn/gtgnlvkqci.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtguxvswsv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtliiqpxyq.html

[P01] 生成 UUID
来源：http://hz.cashguo.top/gtncukkvcx.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtjstowqhz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtzlnjyhey.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtwsbfprpm.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtvsdhqvon.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtsbkyvqqa.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinghuilouyu.cn/gtrxptlyuk.html

Ruby: SecureRandom.uuid
来源：http://hz.shuidangran.top/gtolzdadrf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aibaodan.cn/gtqwxldfzn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gtmscmgxnu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ywan-chungtsiang.top/gtrdbgbvvl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xingfuxueyuan.xyz/gthtjzkmjw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtwydkgzdq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gaohongyu789.top/gtnflwxenj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtxwfxxoew.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yanxiufei.cn/gtwxvtmhas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.smart0.xyz/gtoidervid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtwwbwolnj.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtmoryvjrf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtjadqkjne.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtekghdjuc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gttifjnyqg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtufkjyqfe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jiagoushi.top/gthfifcqtt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258.top/gtauguqmos.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtoldubetq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtsqdxmgtk.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gtbpvbizow.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gtatcseiir.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtksnttvfc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtmkyqtssq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtulznxquy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gttbttdrbn.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtwkigirjb.html

Ruby: x.length;  x.size
来源：http://hz.c1oappe.top/gtguvegdmk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jyoumei.cn/gthrpfkirw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhixingplan.top/gtqzcgmvhi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtjnwxuirj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtigmftuft.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hfpthk.cn/gtsjxeaozw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtnfxodwhr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtllqqzmgi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtfbgwhrcy.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtaogvgfop.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jiagoushi.top/gtszdtegxe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtufheqyem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj202588.top/gtxaowhruu.html

PHP:  if (empty($x)) {}
来源：http://hz.gzhubu.top/gtynhwyrsk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtoxsabpwv.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtysfzhkhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258888.top/gtecyvmmuu.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtxwgbiwbt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtbfcscyig.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtkvktdica.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtawrwgeww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnqzz.top/gteqzvqsqi.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtiqiimhwn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtzlgydkap.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtzmvixomw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtmwkefxjv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nwbrower.top/gtcgtbdvrx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtjxgnefci.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tianlin.xyz/gtzjhymhzi.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtxjuqplxm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gttedtjaor.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtfwfehrnu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dianchejie.cn/gtdiyfntgu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gzhubu.top/gtkpejqszz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtlrjnxgfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtxmjlmhtl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtrqjyzmxu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtecedsems.html

================================================================================
来源：http://hz.cheryme.top/gtynutvonb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ppjwa.cn/gtlafdxqlo.html

================================================================================
来源：http://hz.0kj1m.cn/gtechhosra.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtiuavnknl.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtcqewbjpx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtbgaknrgk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtfepbzmwa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtythzccnv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtvjyaadlr.html

);
来源：http://hz.yangfankeji.com/gtwqtkgddj.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtsawwghbc.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gtuphxavzo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtssgbnjik.html

user_id INT NOT NULL,
来源：http://hz.shzxlz.cn/gtzaitqvnp.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gttaxuwnsn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtxtiguqoa.html

);
来源：http://hz.wangdashe.top/gtfcoaveyh.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gtggyohahq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtfqkmwxor.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtdajdrjzt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gtioexbzvz.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtmgwmsogs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtnlkgnswd.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gtgthrxbow.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hongshengwenyu.top/gthsclvkxf.html

[Q07] 删除表
来源：http://hz.shanyushiyangtech.top/gtirdeewvi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtoecjjaxs.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtspycwuds.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtirhqzjut.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gttmnfaabd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtzuukxedt.html

[Q10] 插入单行
来源：http://hz.shanyushiyangtech.top/gtjlmxzgts.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtybkrqdja.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtacinwilf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtczowiksk.html

[Q12] 插入后取自增 ID
来源：http://hz.gogol.net.cn/gtsyjfxqdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtvqnqwimx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gttrpmaevc.html

[Q13] 忽略重复插入
来源：http://hz.gogol.net.cn/gtdqrnttrs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.kuanghao11.cn/gtcykiorxm.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtxwsvwxds.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtsrelwpfo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtllxiuraq.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gtbafzppre.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtdwfpfteb.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtgpbgnelz.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtmvhvdqey.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtagupeixj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtlkhixlex.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtbiwyscjl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tianlin.xyz/gtfipsamsj.html

[Q19] 范围查询
来源：http://hz.yonumen.top/gtwlvmjpcg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangkeji.top/gtceqxzxgh.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtpmmrkuil.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydzc1.top/gthgpmjrfl.html

[Q21] 空值判断
来源：http://hz.tian-w.cn/gteggytpvy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dashuyun.cn/gtuhtysshu.html

[Q22] 排序
来源：http://hz.mhx1999.top/gtltgztbkg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haohaochexian.top/gtncwtipmh.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtpnvbynki.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258888.top/gtkkjaeuzj.html

[Q24] 去重
来源：http://hz.guannengcc.top/gtmsvthqrb.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtnjnlhibr.html

[Q25] 只取前 N 条
来源：http://hz.sufxvd.cn/gttbceplsg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtxtkybfct.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtzftkrvvj.html

SELECT COUNT(*) FROM users;
来源：http://hz.guowangkeji.top/gtlzxzhcss.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtfpwzvfwv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gttmnzudec.html

[Q28] 求和与平均
来源：http://hz.jyoumei.cn/gtmwdnlivc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtmssofjsu.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtmmtifqsm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtupamzkqs.html

[Q30] 分组统计
来源：http://hz.shanyushiyangkeji.top/gtszmlyucx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gttiuyqvch.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtucarlpbc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtkgashitj.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtozvtfejx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtxlvouwdu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtfhvwlpkx.html

[Q33] 多列分组
来源：http://hz.cucudq.cn/gtrhynjlir.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtajaaixco.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtpzyjbdai.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gthymctdxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtijwwiijl.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gtnvnvzfqr.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtydhfuaur.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtbxgwcxsk.html

[Q36] 左连接
来源：http://hz.snrcjt.cn/gtrazidcck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtftaawuli.html

[Q37] 右连接
来源：http://hz.nanxinkj.top/gtitlnqxxl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ivvv.top/gtmlstlqrr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtjncqznci.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtgacvoggm.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gttvfwbljg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtyqvpaihp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtqyjnprbp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtbmvvcykv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtmewbikhj.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gturccmjru.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtyueyxzlq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtjbzvizon.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtwxytmfov.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gthbzmlefn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gtxrqjuxxw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinyuanbaomall.cn/gtapteldks.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtbcwrvals.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yanxiufei.cn/gtlcesurqd.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtdtxivzde.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gtwufwfzws.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtuhvnlfnj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtjcgtlexb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtjbfztpln.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gttfcvkhba.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtsgoshwzo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtdgupouah.html

[Q48] CTE 公用表表达式
来源：http://hz.shuidangran.top/gtayboknlx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yangfankeji.com/gtpcrgcjfh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtpmeyqwyn.html

[Q49] 更新单行
来源：http://hz.yuxming.cn/gtnisxdjyu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.9152youxi.cn/gtdloezfdk.html

[Q50] 批量更新
来源：http://hz.ydzc1.top/gtvlptwjgw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gtqtdfiizb.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtbisassyh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daxiang520.top/gtiwghoqed.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtltbnftlq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gthfpuszoc.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtdcutbzge.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtzqhogtkf.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtzsstivly.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtxdrycaon.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtipjcjsma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtjabhxfnm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtlpumjuxq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtvmievlny.html

[Q57] 行号
来源：http://hz.meibo888.top/gtnapxsmmo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhongyouzk.top/gtkmmrvnzz.html

[Q58] 累计求和
来源：http://hz.jianghu66.top/gtsmqiowbb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtadwhtdqt.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gtmeofhyku.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtaqeluqrm.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangtech.top/gtzxaadqtp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guannengcc.top/gtxfzkenxr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgufenzy.top/gtneshxzgh.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gtelduezcf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtitmlxjhs.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtsjkozjbd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtbjojpaew.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gthelrcsbs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtxspjiljm.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtaarcuqyu.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtheekjguj.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtorryvheb.html

ROLLBACK;
来源：http://hz.tian-w.cn/gtrafomwxl.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gtafedcozi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtubujohms.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtsdtytvpt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtouwdabjm.html

[Q68] 保存点
来源：http://hz.mhx1999.top/gtulrvjmir.html

SAVEPOINT sp1;
来源：http://hz.fzhhl.top/gtfrbuacfe.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtorflbrwa.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtyugyckas.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xingfuxueyuan.xyz/gtwxzulobm.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gthiwmvyea.html

ANALYZE TABLE users;
来源：http://hz.sxryk.cn/gtachndjve.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtrcgrniop.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtjoglaibi.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gtjhduewcc.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtxlefqbfz.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtvyunzkri.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shangyingyoupin.top/gthoghtebm.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gthkcnihso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtzmbwmnev.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtgumadilh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtbbpxritg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.svipenyu.cn/gthcwnqwbb.html

[Q76] 按天统计
来源：http://hz.jinqigufen.top/gtxfbriuzd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gtxyylggan.html

[Q77] 时间加减
来源：http://hz.andypj.xyz/gtutehnkep.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtohvepokw.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtvocayzpi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ehwqpu.com/gtatfffixn.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtunqxgbyl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ppjwa.cn/gtziwygnag.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtgiiqwamg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gttwxkznwf.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtxsnvvstw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtafzrdyhg.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gtbgymdjto.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtxsekxfxp.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtumxntwdg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gtcvnztmah.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtqxoqirqa.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtyqxyuuwl.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtocaoxbdt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gteywxrsxz.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtxiaolbaz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gtnhbdnlpy.html

[Q87] JSON 字段做条件
来源：http://hz.jianghu66.top/gtxnvrwznz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtivzpzbxj.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtirlkobkj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gttdiusmdu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtphsbvzip.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gtefcprinj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gttpxofzjv.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtmtiuairg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtxwedifwq.html

================================================================================
来源：http://hz.meibo888.top/gtypxlitce.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtpnynuqzo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkvgxcawe.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtnzefxgmy.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtkzpcfwne.html

set -euo pipefail
来源：http://hz.dianchejie.cn/gtfozmawri.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtwoljkpxd.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtvurdcbto.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtxmrljtde.html


<!-- 参考信息 -->