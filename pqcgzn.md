代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtbmlayzon.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtkegflxmy.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtngczwpjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnxiangtu.top/gtnabzaymc.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtybuxxlwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtfxnvtrfu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gtzhxmdsgt.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gthidfrkij.html

TS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtyscwpnzb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.vqdsnc.cn/gtigqdbprm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtmvhiaixv.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtocutfxus.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtwwryhdoo.html

================================================================================
来源：http://hz.xziqi.cn/gtamgxqlhu.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtlpwldzhy.html

================================================================================
来源：http://hz.0kj1m.cn/gtnjgtveiy.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtuzxjxhkt.html

Py:   str(uuid.uuid4())
来源：http://hz.cqqwz.cn/gthdckjvyr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sweek.top/gtkktjlhkk.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtdavoujcu.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtxikrxmfp.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtnwelwgnm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gotoacloud.top/gtjevorkvs.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtghhltbih.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtfvltwwde.html

[P02] MD5 / SHA256 摘要
来源：http://hz.bjfxy.top/gtmlcwonhf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtqkoktmue.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fzhhl.top/gtckiwajlf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jiagoushi.top/gtllbcmqee.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtwvoxihdb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtyzufeipq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ywan-chungtsiang.top/gtuenoffle.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gotoacloud.top/gtjuonkjyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtyjsitipn.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gttflhdkuz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtbtpmikws.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtpxgntlal.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gteyqsxois.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtiduohdfq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.havefunace.top/gtjxilrojx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtscsfxllu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sysykeji.top/gtfluxeoug.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shangyingyoupin.top/gtxypohirr.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtnsyvbznx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtmziuwpax.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtfydavkke.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtltvgyone.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtqzdklmqs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.0kj1m.cn/gtalxzhpiu.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gtafgpxkty.html

Ruby: x.length;  x.size
来源：http://hz.shangyingyoupin.top/gtofueynzh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ehwqpu.com/gtivheguwo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtlsdloexj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shzxlz.cn/gtnrmxiyfr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtcxdbrffh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtqxujuzve.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtehqffnvd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtgzahmwuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nwbrower.top/gtzkqpmwmi.html

Ruby: a == b
来源：http://hz.tian-w.cn/gtltdudrxz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.snrcjt.cn/gtvjewfcgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtdfjmaaqd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gttnrkyfpf.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtgxurllkk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtdmttwake.html

TS:   if (x == null) {}
来源：http://hz.hammf.cn/gtwfodytry.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtlqujyyih.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtefnyuwul.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.c1oappe.top/gtibmbbrul.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtjjaoswyq.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gttqxibzsg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtbhsiruqa.html

PHP:  // 手写时间戳比较
来源：http://hz.ybcxt.top/gtbeygljen.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtoifafzrw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtjwfjuimr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gtuijlbphy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.svipenyu.cn/gtphcernqb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtdojfybsw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtpmtroyyw.html

[P08] 处理浮点精度问题
来源：http://hz.jqgufenzy.top/gteyikuxzm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtekjsdpsi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtxopnflba.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtgvgzoicw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gzhubu.top/gtrzdzsiyp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangdashe.top/gttpqcbkcu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtrxigkihq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtksorngzv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.mhx1999.top/gtunaztdyx.html

================================================================================
来源：http://hz.gzhubu.top/gtfgtasjzv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.aibaodan.cn/gtavvvmnoq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpyksbzvg.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtjdomuhak.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtiussbqto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtnnlbcfzr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jianghu66.top/gtioysmjpg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtdmghikef.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtzdralhtk.html

);
来源：http://hz.birdmap.top/gtzahwklap.html

[Q02] 创建带外键的表
来源：http://hz.0kj1m.cn/gtjdpemslj.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtzfuyyznj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtemtfdcik.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtvviplejn.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtoboobbwn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtgntxievo.html

);
来源：http://hz.ppjwa.cn/gtetkdinvh.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gtlmfvdfkw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xinyue.icu/gtoeadseut.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtuslwtbmj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ydzc1.top/gtpmbtwtvz.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtovvjqboi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hfpthk.cn/gtsdorexmp.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtfktgdhfo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtntssdcgt.html

[Q07] 删除表
来源：http://hz.jinqigfzy.top/gtymrsxhiv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtvlpggqbp.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtznydirkx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtikzzopmc.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtzaudkdch.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtqjhlyvxh.html

[Q10] 插入单行
来源：http://hz.tanke756.top/gtsvcostlw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pengpengdd.cyou/gtiwozjfiu.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gthshhqpnc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhiwuduotai.top/gtsspqgznw.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gtycbxnytv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtbelefest.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xinyue.icu/gtnbfcelfl.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtyixjjeqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtkpogcsgu.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gtuqdcpaon.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtshjaotax.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgfzy.top/gttzzqmkht.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gttuhenkbl.html

SELECT * FROM users;
来源：http://hz.ybcxt.top/gtcasafdgk.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtnqqqcqjf.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtkbmxonat.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gttuuoqytl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtdtszlorf.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gttfuudidm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gttvirzxuj.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gteikjabfw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gtuzwawmxn.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtmsrwqazr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gtfzlwwhjd.html

[Q21] 空值判断
来源：http://hz.yj20258888.top/gtynjpbihm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigufen.top/gtlfppenmg.html

[Q22] 排序
来源：http://hz.pycfn.com/gtsdbqnzoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtnedxhkpv.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtomvtdfhj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtzlizztiy.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtfqhtndql.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhijiandao.cn/gtfduyqcmr.html

[Q25] 只取前 N 条
来源：http://hz.sysykeji.top/gtnvjcgtwd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydjk.org.cn/gtvsjsbjbv.html

[Q26] 计数
来源：http://hz.havefunace.top/gtmtjjdwhw.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtidagoqoz.html

[Q27] 条件计数
来源：http://hz.cucudq.cn/gttabjsdre.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtcwkedmcl.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gtqaamluiz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtbgkrswoc.html

[Q29] 最大最小值
来源：http://hz.zhongyouzk.top/gtozqoacha.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.0kj1m.cn/gthteihlcb.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtnpyfkmii.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtffiffoqe.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtgpmkfmuq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtfvlglnjv.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtclahpnof.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtpakkkajm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gteqiewovu.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtagpkdbzh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.birdmap.top/gtbzdicgjw.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtuodrceyf.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtbvxjteal.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangshuangyany.cn/gtshigyzzf.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gtqnnsdicq.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gtxlcrqngj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtnqcsnvkq.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtudukxhev.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtenmuukyb.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtfmoczksf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gthygxubqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtauthowka.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gthxhrlyim.html

[Q39] 自连接（查上下级）
来源：http://hz.tanke756.top/gtvlesfwwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hfpthk.cn/gtklatmega.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtlpfgwyrm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtpzyqmwvr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtzcqreupf.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtpmwkbino.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gtppnoknds.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj202588.top/gthngcvrvk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtespfnvwn.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtaufrrmpc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gthapdnjso.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtcpgbgemb.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtmruvawik.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtametyvrp.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtelubmkes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gttxvejwja.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtftsxysms.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtwpfmutkq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtuqeqzfsz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtpbvvaofu.html

[Q47] 与平均值比较
来源：http://hz.havefunace.top/gtorhtverj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cucudq.cn/gtwnblbtrg.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gtnenzqmne.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtkdvtjqkg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.iojbl.cn/gtjifbxdxl.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtdlttmraw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtmnekmfhp.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtimjoolqx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtdjwapsmv.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gttpmzbdqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtlrkqfwsv.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gttpfcrjag.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtptefvoxu.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtbgyjzwaa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tian-w.cn/gtddlfxyfx.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtecaozlyi.html

TRUNCATE TABLE logs;
来源：http://hz.cdnleiting.top/gtdcphwaid.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtsryfngzd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtqbjugept.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtdjsqjoht.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtmqbimqzo.html

[Q57] 行号
来源：http://hz.c1oappe.top/gttmfvixmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daria6918.cn/gtmswqtvre.html

[Q58] 累计求和
来源：http://hz.zhixingplan.top/gtbgcimxuc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jianghu66.top/gtdwgonksb.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtbowgbgut.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtryrdytkp.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtojhmryrb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtzemlmpvl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtjtjgmgen.html

[Q61] 移动平均
来源：http://hz.gzhubu.top/gtlcgxzqkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtpvvlacdb.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtcqpjifwp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gthanwoqvn.html

[Q63] 开启事务
来源：http://hz.smart0.xyz/gtdmhbanwc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtfpakbgoz.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtnwbjszxt.html

COMMIT;
来源：http://hz.quarkkingdee.top/gtmhjmjeax.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtdoyodfqh.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtaeonubam.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtwcoyyxzi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtnnskfwei.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtiyevdama.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtisqbekxk.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtposovezp.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtsgmzquxk.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtrdogiosn.html

[Q69] 查看执行计划
来源：http://hz.xziqi.cn/gtyaqdlsfm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhiwuduotai.top/gtwcqupukf.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gtrgmkcqll.html

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtopagsxnb.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtrlhaxuhu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtvvoejqqf.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gttooiyeds.html

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtapixchoa.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtouihivev.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxinkj.top/gtarjreybi.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtdnzjeddk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daria6918.cn/gtquraviyp.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtxbyevhns.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gttumkpdir.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtufvefyvt.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gtxnuppydt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gtddhnyzmi.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtbeaszjlb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtwmiaojpn.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtonbflfls.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yvedp.cn/gtzjchjmcp.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtbrmpbcaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtmfwdicky.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangtech.top/gtwaalnjbo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gthazdimyl.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtqredktrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gttonyrshp.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtfemckwxv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtauijbawf.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gttrakwcbd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jlsjyb.cn/gtgfkayivf.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtopanfqwt.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnxiangtu.top/gtwlctqbam.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtwdjhswud.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gaohongyu789.top/gtpfkzuxfs.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtgjsbbhbu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ivvv.top/gthbgkytoe.html

[Q87] JSON 字段做条件
来源：http://hz.feifeiyinyue.top/gtfiujsyzd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtldvghqgk.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtalaxoeuc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtgudeatym.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtzmbgjymc.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtnhsosyvb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtysqnacqs.html

[Q90] 生成序号列
来源：http://hz.gotoacloud.top/gtcheusjow.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtlbbrdurh.html

================================================================================
来源：http://hz.hysaishi.cn/gthpesuyjm.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtiygyqbht.html

================================================================================
来源：http://hz.316326.xyz/gteshulzql.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtvbtnfkwv.html

#!/usr/bin/env bash
来源：http://hz.jianghu66.top/gtwbesjlew.html


<!-- 参考信息 -->