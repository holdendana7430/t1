代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtrqugzpnc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ywan-chungtsiang.top/gtfpdfaaul.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtcfeqvtwf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtuanexwgk.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtlmqfzvpa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gthajsyduf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xinyue.icu/gtkoemmdne.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtajhjcfjh.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtqtrodrye.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtaikbgixi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shzxlz.cn/gtiwgartbh.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtxuurxutg.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtcjkeuuzq.html

================================================================================
来源：http://hz.sweek.top/gtvahvkvcm.html

P. 常用工具函数
来源：http://hz.hysaishi.cn/gtehphvlsw.html

================================================================================
来源：http://hz.daria6918.cn/gtsasmuvmf.html

[P01] 生成 UUID
来源：http://hz.zhongyouzk.top/gtfxhvvwxm.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtlbiqvbwq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tanke756.top/gtyzlpcatk.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gthjftdtfo.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtypdnoqzq.html

Java: UUID.randomUUID().toString()
来源：http://hz.52xcode.cn/gtrxgbprbn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhixingplan.top/gtncnngmbv.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtgzdiybag.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yangfankeji.com/gtsuluwfxz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guowangkeji.top/gtidvkkmkn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gttqgxcpuh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jiagoushi.top/gtkdiuscdi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtrdxqksuu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtxnmkzyxx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtaxagdrqa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xingfuxueyuan.xyz/gtngrrifwp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtiqindsxj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtpxvhunzb.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtlcwymwvp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtaowllquf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtzfuncqxi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtediexzkz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gthctvnfbk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuanzx.com/gtzevhuufs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pycfn.com/gttqdqvspn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xingfuxueyuan.xyz/gtzqyrtnyl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhengqikj.top/gtzgxzcpuq.html

[P04] 求长度
来源：http://hz.tian-w.cn/gtjsvuphgo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtffnlqumn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtzhjfonfa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtsjmzaenz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtmsmafwnl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtqzagfnwv.html

Go:   len(arr);  len(m)
来源：http://hz.ydzc1.top/gttlkryaoc.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtrrtcnkny.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.iojbl.cn/gtjmfupnia.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gthhkxlzbq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.c1oappe.top/gtywbxawjj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtjfkamhby.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtbasbqqoq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtxvwtrics.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtzyebmeoh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gteclrnvek.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtyhrxtvmv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shuidangran.top/gtecewkpwy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtoqguetrr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtaibrppjx.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtdxoesgaw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fengsongda.top/gtcqicopfr.html

TS:   if (x == null) {}
来源：http://hz.0kj1m.cn/gtcfmnumbf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtpgqymjrj.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtmjhiohjo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.birdmap.top/gtfblwtieo.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtiotauqzt.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtanmlftqn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtfiynvvpb.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtsssjnqro.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtvfnwnxih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtdqtsfcvj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtukllxisg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigfzy.top/gtdyeolrow.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gthqkbqglf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hongshengwenyu.top/gtrjhzmgiw.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gtloykqjga.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtipbdfnub.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cdnleiting.top/gtqetjxyqj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtfbaxmavj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sweek.top/gtmytsajyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtmbnpwrws.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daria6918.cn/gtvhhuoqvo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtquadieaj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtadwluwmy.html

================================================================================
来源：http://hz.pycfn.com/gtrpogupen.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daxiang520.top/gtlfgpevrn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnxjhhxlc.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtcvjzgwqp.html

CREATE TABLE users (
来源：http://hz.dashuyun.cn/gtrhvwbxat.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtnijhrebz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtjbqazmso.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtylcgsudi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtmxshpbls.html

);
来源：http://hz.pengpengdd.cyou/gtqlybnqik.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gthsvohfde.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtqujycscl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtubhnxwdn.html

user_id INT NOT NULL,
来源：http://hz.redwolf501.top/gtnemndvme.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtguhrgdap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ivvv.top/gtagzcrjaf.html

);
来源：http://hz.chenjidiqi.icu/gtytsfjzqc.html

[Q03] 增加列
来源：http://hz.yongpay.top/gtyplkdykc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtgvdnbhss.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtvwvpdqwk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtspupbjnh.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtnyjejkqs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.316326.xyz/gtpgfzzsly.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtfcbjqyqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtodghlpru.html

[Q07] 删除表
来源：http://hz.jqgfzy.top/gtsscqdhok.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gttafnvqdb.html

[Q08] 创建普通索引
来源：http://hz.jiagoushi.top/gtxqwovsig.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gtffxgsqql.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtczkkycgf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gtfubltjip.html

[Q10] 插入单行
来源：http://hz.pycfn.com/gtjnglarfb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtabiviaog.html

[Q11] 一次插入多行
来源：http://hz.bjfxy.top/gtsmmsrbsq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.smart0.xyz/gtwauwfmhl.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtujcyxibz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gttztxmuzb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtbgcjhlta.html

[Q13] 忽略重复插入
来源：http://hz.gogol.net.cn/gtfuzkgeuz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtrlnfcyqh.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtykbgoyiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtsbwstwwk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.52xcode.cn/gtoytabzkb.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gttbmlgwdj.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtzjqwrthh.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtmpcyxmad.html

SELECT id, name FROM users;
来源：http://hz.aibaodan.cn/gtogijddec.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gterfhrdjl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtouepfqlw.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtribraqbw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gttmcbcnhr.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gthcpcpkkh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtmdxlwrpx.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtvqzynylf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtzjbrvabt.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtqisrkwfg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtoevcvsef.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtcjsitkdt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xinyue.icu/gtkdoujwci.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtimzkiuxn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenzaomai.com/gtfiuebtth.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtweaypnbn.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtfwzqtxbj.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtkdbdkjnx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ehwqpu.com/gtilyuywhb.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtlusfoejy.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtqkhigzny.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtsmbtrykz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.iojbl.cn/gtfzfdanrd.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtliddcjaq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cqqwz.cn/gtjunptout.html

[Q29] 最大最小值
来源：http://hz.cucudq.cn/gthbegjwzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhengqikj.top/gtxeccyouw.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtmzilnojf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtyzycvmos.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtymzxngzb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtjviomivs.html

[Q32] 分组拼接字符串
来源：http://hz.9152youxi.cn/gtiitiqfyu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtialfsose.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtdlwwsmvp.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtbiwzdxnh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gtuaxjhvvp.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gttvoxtiwp.html

SELECT * FROM (
来源：http://hz.hysaishi.cn/gticxffcsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtjopelxfx.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtzplytncg.html

[Q35] 内连接
来源：http://hz.cdnleiting.top/gtgwrhjyhy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtbvsbrhfe.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtialrcdpd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtevrqcnuy.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gtahgbbdae.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtygrteags.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtxwemzuri.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtzjxigdjp.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtfqzltzrz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zdqjudy.top/gtnfcucfer.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.316326.xyz/gtdirdladx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258888.top/gtdmrlupyn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtlunnrzlf.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtbtmfupuh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtjdsuptdz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gtsbwhjymf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangtech.top/gtzjqqwqlg.html

[Q42] 连接条件附加过滤
来源：http://hz.gzhubu.top/gtwqowbktc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgufenzy.top/gtvmrijpix.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ehwqpu.com/gtrnosdpde.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtkeezgibz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtdsivjdoa.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtutnblzfe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtgozdbyyh.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtncobywxn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtzfnunefs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtlekzltll.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gthfoecprw.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gthfloomjb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fengsongda.top/gtlblpzief.html

[Q48] CTE 公用表表达式
来源：http://hz.tianlin.xyz/gtfqgldbca.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtjiljaaee.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtsthawhiu.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtgkdifoai.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtcoufojyk.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtudljvyhd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.svipenyu.cn/gttfytnick.html

[Q51] 用子查询更新
来源：http://hz.hammf.cn/gtehetjzle.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtnwspikoi.html

[Q52] 删除指定行
来源：http://hz.ybcxt.top/gtfiezcprv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtrxywjwig.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtkkuymunl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gotoacloud.top/gthlqybpxx.html

[Q54] 清空表
来源：http://hz.gotoacloud.top/gtcimkcvcs.html

TRUNCATE TABLE logs;
来源：http://hz.cashguo.top/gtcbrwgbne.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtklasnkrh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtqmcomlhu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.bjfxy.top/gtsagrvbzc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtqfrurcey.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtpsmvoyuq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtyeytuvgn.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtacwnikdu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gtcyyfojkp.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtvrdallik.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtbtmyizzw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtosvqvjlf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.quarkkingdee.top/gtgrgxknnu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtouwocaga.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtpsbhmmvx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxuanxn.top/gtvijxaxgx.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gtllrqpukc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtkxvbtnwk.html

[Q63] 开启事务
来源：http://hz.shanyushiyangtech.top/gtqgdhvgsn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtwpxzweek.html

[Q64] 提交事务
来源：http://hz.nanxinkj.top/gtweohppbu.html

COMMIT;
来源：http://hz.aibaodan.cn/gtvknushif.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtvigzqoud.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtlqzbjhiu.html

[Q66] 行锁查询
来源：http://hz.ydjk.org.cn/gtkqtuztiy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtrqmnjgka.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtgbuuoufe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tianlin.xyz/gtxrewgfvy.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtmrhrowaw.html

SAVEPOINT sp1;
来源：http://hz.ybcxt.top/gtdalvieov.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gttpzfmjzk.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtnffgasoj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtordgwonk.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtwflszakc.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gttaskegkr.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtdncxoueh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtvlkvdogf.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtdpgpuobq.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gttvfzuxdf.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtsclmismp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.haohaochexian.top/gtkvwfaryj.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtuxmkywhb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtweamrgfj.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gtbhoxaftu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtzalenlxo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gthkglyock.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtvhapuczn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtjodwzbfx.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtijzdikuw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtmlvystph.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtweioytof.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtfuxxocjm.html

[Q79] 字符串拼接
来源：http://hz.shuidangran.top/gtgffdazqb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtddzdmdvu.html

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtnqemwqer.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtxnkqgrej.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gttkdxsbrf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpdlatevf.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gtwlugkibd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.daria6918.cn/gtrulppoek.html

[Q83] 大小写转换
来源：http://hz.shzxlz.cn/gttwizxjbv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtzgjvzfou.html

[Q84] 去除首尾空格
来源：http://hz.tian-w.cn/gtqbmrzsjb.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gthmftbjwt.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gtadehmghv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zdqjudy.top/gtobiaqqdn.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtmygeuhlq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtyrncrahv.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtvlkqtwxh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.havefunace.top/gtwldefilc.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gtcjhaksge.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtpolnrdyx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtkgrxloeg.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtvobuxlgt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtkiuotvvo.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtokuvljik.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtlitkucjm.html

================================================================================
来源：http://hz.aibaodan.cn/gtkmurhcxk.html

R. Bash 专题
来源：http://hz.yongpay.top/gtwzdxjywf.html

================================================================================
来源：http://hz.nanxinkj.top/gtlgdjutmv.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtrusiplom.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gtgmgwfyfw.html


<!-- 参考信息 -->