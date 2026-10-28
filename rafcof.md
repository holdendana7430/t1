代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pengpengdd.cyou/gtavptslms.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtfaabwzzp.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtgisizcts.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtsxzmtcsj.html

[O06] 使用进程池
来源：http://hz.jinyuanbaomall.cn/gtkkyqpigd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtlcennrhd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ywan-chungtsiang.top/gtzbslnuvf.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtkawjrndp.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtpykqhyby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gttujzqyqx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.aibaodan.cn/gtcbvdsmut.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtgxyqnqfc.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtpdyxydme.html

================================================================================
来源：http://hz.ydzc1.top/gttfgvjrxa.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtpfvzknkg.html

================================================================================
来源：http://hz.cashguo.top/gtbmtnning.html

[P01] 生成 UUID
来源：http://hz.kuanghao11.cn/gtstmbebfp.html

Py:   str(uuid.uuid4())
来源：http://hz.daria6918.cn/gtdgbrnwfq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtjgilwntt.html

JS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gthwcnaumu.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtrlpmglzk.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtwnknspmp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtrjlxswox.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtklzlxzvi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtmfngacqh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yangfankeji.com/gtyotofnmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shuidangran.top/gtbdntifyb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tian-w.cn/gtsxrszuil.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtkgusaioq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtlmumcitv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtbdczshtw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yueranfly.top/gtgbgxlcxo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shuidangran.top/gtxorsmooe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtojfxyjzy.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtbhwdefre.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtlszgvvhi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtkxczvraq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtdgbysndk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gthztekank.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtrbgxrhcg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gtwcikamcf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258.top/gtrgzvxxvw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtjbvvxdqd.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtdimvldua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gotoacloud.top/gtsojwzjiy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtdivhylvr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gthohbkazx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gthuoiitht.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhijiandao.cn/gtsrlcjstj.html

Go:   len(arr);  len(m)
来源：http://hz.tian-w.cn/gtjpytjfkb.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtcnihunjz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gttcysbsxm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtecvoulis.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtnxpwqsgj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gtjcifqgii.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtiewekuqi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gteqvihfig.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cucudq.cn/gtwyehikgm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtjpmyibga.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtlknnwryt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtxuzhbkea.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtnqprjouw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtotdqfren.html

PHP:  if (empty($x)) {}
来源：http://hz.zhiwuduotai.top/gtwldbbvnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtbclzufuq.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtpiobvddz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtyvmdltln.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtgotnalfz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtogqqhgiv.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtvjxhzrcb.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtrvktijbx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gttsqclsam.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtvwygvohv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtsivdjzrw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtqbdvpwaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aizwys.cn/gtmctbovxq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinyuanbaomall.cn/gttjjbzpdr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cheryme.top/gtanznjnpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtwgrwylgk.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtyshgbvbi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hfpthk.cn/gtlfjphzlp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtzuvlummn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtstijhqnt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtulfgmnjh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hongshengwenyu.top/gtpwurnyxi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtslkqmzxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtmnremtnk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtmitxfoeg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjxcprjdx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.smart0.xyz/gtsvuhqwyz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvgjbwhkd.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtkmmmjchb.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtyextaede.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtaiaknjci.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtfkwupunf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.birdmap.top/gtcdvvbodb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jlsjyb.cn/gtoqltwvgy.html

);
来源：http://hz.zhaomingkeji.xyz/gtcwzcjhvj.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtwaifbjcp.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtzibyywsc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtvcsklmus.html

user_id INT NOT NULL,
来源：http://hz.redwolf501.top/gtoahrnfbs.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtglenbcdd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtkxygbvfk.html

);
来源：http://hz.shanyushiyangkeji.top/gtblkeblol.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gtkmvykzaj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtydwwmdhm.html

[Q04] 修改列类型
来源：http://hz.jinghuilouyu.cn/gttyhkytzx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtccjdicnz.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtlqdgvaqh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtnhhyqmcj.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtdygpvsmn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gtqbfwpqkq.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtkeexcuum.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtsjgdktbt.html

[Q08] 创建普通索引
来源：http://hz.xinyue.icu/gtnrflwasf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtmvvnqoym.html

[Q09] 创建唯一索引
来源：http://hz.hnxiangtu.top/gthjxdwmek.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtbvytovlm.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtmohxngpw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtupjviodd.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gthzhxkulc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dashuyun.cn/gtbqfzaime.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtsqbzbjmw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtpulefhts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gtdflxhquq.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtvtyadxyv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenzaomai.com/gtadbcqqgi.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtiulclnpp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtfaoqmpru.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtocjytiou.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gtyfiljywl.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtmijsivnx.html

[Q16] 查询指定列
来源：http://hz.andypj.xyz/gtdyovauev.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtiumttcwv.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtvydfktkx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinghuilouyu.cn/gtzdrivcyh.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtuvyotcrb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtzirlqvby.html

[Q19] 范围查询
来源：http://hz.nanxuanxn.top/gtwasumrpl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtaixcrfrz.html

[Q20] IN 列表
来源：http://hz.yuanzhike.top/gtmeauymct.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtqvzzqfjl.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtgjqkkwby.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtxakjynnm.html

[Q22] 排序
来源：http://hz.xuetiantiany.cn/gtmquzflgq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtkwvwqlla.html

[Q23] 分页
来源：http://hz.xuetiantiany.cn/gtrhewftbb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtlcelflok.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtsycuwcbm.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtwvtlgatd.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtoqygscak.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtyfrabmmr.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtsrtcqfvu.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtjdczdffw.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtuaklsare.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtmmqqbaae.html

[Q28] 求和与平均
来源：http://hz.jlsjyb.cn/gtajjyxfaf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtxybhgkhl.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtqhasqssn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtwwivtero.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtmwmfmrgu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtwtgqbfds.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtuvndfayv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ivvv.top/gtdqapxilc.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtkzxufxfu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtcddpxcff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gtdyfrozll.html

[Q33] 多列分组
来源：http://hz.gaohongyu789.top/gtubitnnlv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtygzngflm.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtkxfsvwsz.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtvgkwkdno.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nwbrower.top/gtyymyemwp.html

) t WHERE rn = 1;
来源：http://hz.tian-w.cn/gtgojxbfyz.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtjncosdfj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtoxnydrnp.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtfwvczxsx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtkxoqmiic.html

[Q37] 右连接
来源：http://hz.shangyingyoupin.top/gtyghvsuzk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gtyqfpdofv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtgvbknqcs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gthxxafwfo.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtxjuwicaj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtfhxniiau.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtgwoobbxz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gthwspibmg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtjfsjbknv.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gtzuuegeqo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gtwiyuulnx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtujqcwmjw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgfzy.top/gtrdlfgmwk.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtvnlwifmb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtelelturm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtnikqxeii.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtdvllnysj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtlsdakzjb.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtgahzuzfq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtkybzkfxh.html

[Q45] EXISTS 判断存在
来源：http://hz.meibo888.top/gtmuqvghks.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtagxbqlxo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtoekcxrwo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtnvtwbrik.html

[Q47] 与平均值比较
来源：http://hz.shuidangran.top/gtyxmzewyp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.snrcjt.cn/gtnwshvfsa.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtlbbvcske.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtwdcblwme.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtsojqlmae.html

[Q49] 更新单行
来源：http://hz.shuidangran.top/gtrurtzvfs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtrqlcemzs.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtcrmohnxt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtphvlcmms.html

[Q51] 用子查询更新
来源：http://hz.daria6918.cn/gtfybjwnka.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gogol.net.cn/gtawrkcpth.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtahmzzxgk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenzaomai.com/gtaegdodww.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtykdsdkeo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtrxeujwqe.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtaslhxdvd.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtzkroaqiq.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtqffmbxsd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yongpay.top/gtlwsfknez.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jlsjyb.cn/gtyaqyzueq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtynjpzvum.html

[Q57] 行号
来源：http://hz.yanxiufei.cn/gtopsaifkh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxuanxn.top/gtjywatkvb.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gtvnnqdibo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtzxcugdbt.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtbisngbli.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtrrkfqagx.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtpwzjuerh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtoubphmbe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtyzgveugv.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gthlnisdgf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtpshpmcbo.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtjjzgkthx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtianosteb.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtkghlyxsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gtrxncixqm.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtxkjcholf.html

COMMIT;
来源：http://hz.zhixingplan.top/gttzkiifuo.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtpycbggtf.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtjmaisqgv.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtuzyqahtd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gticzndhhd.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtjbwbwlie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtenvadvok.html

[Q68] 保存点
来源：http://hz.mhx1999.top/gtvgckbjwf.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtwvyckkjc.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtzrccpyka.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gtpviuictb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gtfuamgtyl.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtkcwkzilb.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gtwioncygi.html

[Q71] 查看建表语句
来源：http://hz.xziqi.cn/gtobugthir.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtixnkfnmr.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtimhrbnal.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtzijltvdt.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtnkcglusv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xingfuxueyuan.xyz/gttretkcnf.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtjenduwuq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtbfwxfugs.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gtesoeeqql.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtxkxpjxfc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.kuanghao11.cn/gtyazbjurg.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtirgvtmuf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtjjapiecl.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtyntdnkjw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shangyingyoupin.top/gtwewurssd.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtfxcfplps.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtajjlokxn.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtsfiwziea.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuanzx.com/gteaanisqg.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtfpgicwza.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtggmmpgyx.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gtbxcpgnwq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtbgpxavdv.html

[Q82] 字符长度与字节长度
来源：http://hz.havefunace.top/gtvxjiikhl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gtzeyazmie.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gtmoldbpth.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtmocyrfru.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtwoxeevbl.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtdvwwxqcd.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtarvzydwk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtbltjarqs.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtocpnagaf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cashguo.top/gtdxompchs.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gttymqgjon.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtjiplhsza.html

[Q88] 行转列（条件聚合）
来源：http://hz.jlsjyb.cn/gtykwbbwqo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtcdvmyupe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cashguo.top/gtvrkmrodr.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtewwoydeb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtaessxiny.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangkeji.top/gtaltshicc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtynopjszf.html

================================================================================
来源：http://hz.ybcxt.top/gtjeddqdmw.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtmsozlnya.html

================================================================================
来源：http://hz.dianchejie.cn/gtxrghnjkf.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtpfjeweql.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtotdejhey.html


<!-- 参考信息 -->