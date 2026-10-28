代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtjefgphnv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sysykeji.top/gtibacftzd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.52xcode.cn/gtufplsepb.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtqajklxbx.html

C#:   Parallel.For
来源：http://hz.cdnleiting.top/gtaxybmbtp.html

================================================================================
来源：http://hz.zhixingplan.top/gtdmltzelr.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtccsrhnqy.html

================================================================================
来源：http://hz.chenlongwang.top/gtpcgklzkx.html

[P01] 生成 UUID
来源：http://hz.sxryk.cn/gtwfpwadxy.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtikdjxywt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gttocetwyf.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtedpkzyob.html

TS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtmklodxrb.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtjycwoxzq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sysykeji.top/gtvnyailwm.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtgaifbvjf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aizwys.cn/gtmvfpvbmr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.quarkkingdee.top/gtamdgkumd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nwbrower.top/gtgbomgmzl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuxming.cn/gtkptqvuuf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtitzoarke.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtrcuidhif.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtsbeepopn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtivqucafj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yanxiufei.cn/gtxsfjvebe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gtzjllzvoh.html

[P03] 生成短随机字符串
来源：http://hz.zhixingplan.top/gtdplzkmkn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhiwuduotai.top/gtpzazopla.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinyuanbaomall.cn/gttokmfdlb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtzsptujdi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtomrxonqo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pycfn.com/gtjxymxbez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtneaoooxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gzhubu.top/gtfjiqzgmv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fzhhl.top/gtsdgsoirl.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtksdqbatg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtavhocrjq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtsrtfxtlx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtfmdqjkok.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtlarkdfnh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gthkchwwoy.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtmhgvptxu.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtqricftdc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zycfv.cn/gtevwfrswc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtzxnpxypn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yvedp.cn/gtypwidoxq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtfssolcqz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtcwzmpubj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gttcuunqyo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gteacetlni.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.andypj.xyz/gtbumjlrle.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtobjlexmt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gtpwixfguh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gttazccwjc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtsxlovcej.html

PHP:  if (empty($x)) {}
来源：http://hz.hammf.cn/gtpiupjooy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tianlin.xyz/gtrnrgeygc.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gttwhgxnee.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tianlin.xyz/gtofekkszt.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtjrfavjer.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xuanzx.com/gtumydnavb.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtfvennzkt.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtkgyqfwrv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ivvv.top/gtflygtrid.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtpxqisglc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtptbzujrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtdnonncyn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258.top/gtniqboxiz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gotoacloud.top/gtceyjujaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangtech.top/gtknqzztpj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtzoqmxyyd.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtwnmxfves.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.redwolf501.top/gtuzqwvzrs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangdashe.top/gtmbhpgacp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sxryk.cn/gtugkhicpm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtpkimpeiw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hongshengwenyu.top/gtrhrlgmar.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.haohaochexian.top/gtowtxinbn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jlsjyb.cn/gttyklqhqv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtavnollhb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttswbfmvb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtfrvxiadh.html

================================================================================
来源：http://hz.chenlongwang.top/gtlasgtock.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtvzcdyzqd.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtvfukajwm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtlwjcihkl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtvoooharx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gtacqbmixl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gtlpkrboqg.html

);
来源：http://hz.tianlin.xyz/gtdslstbis.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtsenmsaig.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtvyknwqoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtoqntqtib.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gttkxyptpe.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gtvplugsby.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtuaagtnki.html

);
来源：http://hz.cdnleiting.top/gtovgzxcjt.html

[Q03] 增加列
来源：http://hz.dianchejie.cn/gtpmnebfoo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj20258.top/gtfzkzzcrm.html

[Q04] 修改列类型
来源：http://hz.mhx1999.top/gtdtkfapql.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shuidangran.top/gtasuscmpk.html

[Q05] 重命名列
来源：http://hz.vqdsnc.cn/gtiptcucdx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtolkmxlqj.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtzzayyhoc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtkjwcxlgg.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtfgtbnlek.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtyhzajnqp.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtdyrwgmff.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtntegdeew.html

[Q09] 创建唯一索引
来源：http://hz.wangdashe.top/gtbhzgfzeu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtgjnnfprr.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtsdicelme.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xylfe.cn/gtvlhjhhnb.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtlzuenqvk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtgqdcojty.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtazonmxeb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gttqbaokka.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dashuyun.cn/gtjnrymwfu.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtygqizelm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gthdlrkrnk.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhengqikj.top/gtsppowrxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtfeyxuchl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtkgbfjiyg.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtteqhcizg.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtcbacypek.html

[Q16] 查询指定列
来源：http://hz.chenjidiqi.icu/gtkyabjlgm.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gttwxlfoev.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtstxeuezk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenlongwang.top/gthssswxjk.html

[Q18] 模糊匹配
来源：http://hz.xinyue.icu/gtcaogucpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.vqdsnc.cn/gtjwsmzdez.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtjjyqungq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuanzhike.top/gttsrrdwfm.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtkcfnoibk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtrpnfdoez.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtzylviikz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gtegvahqsr.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtspwasbns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtzvsiudxc.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtdvnyarpo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtakifzpae.html

[Q24] 去重
来源：http://hz.nanxinkj.top/gtjkaxqgxh.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtpujsfbhk.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtwbgsnyxp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtdyypygyt.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtfbilrkny.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gthfaaijnv.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtvmxqyufg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtpucyltvo.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtmufrhyau.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shuidangran.top/gtydupqynk.html

[Q29] 最大最小值
来源：http://hz.dashuyun.cn/gtmgwptuym.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.haohaochexian.top/gtedgjvknk.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gtmmdaheae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtsxbhpzqt.html

[Q31] 分组后过滤
来源：http://hz.hysaishi.cn/gtbtoqmxjm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtusdfwzgg.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gtlidnbpju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtgnjoraua.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtcdrtwtty.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gttoetwewq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtwwznxiax.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtfsktemjy.html

SELECT * FROM (
来源：http://hz.shanyushiyangtech.top/gtayajpymj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuanzx.com/gtwvcvyjnu.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gtsouxcdct.html

[Q35] 内连接
来源：http://hz.xuanzx.com/gtsorodpen.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtangkktpr.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtojwgalvc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtwzdbkqxp.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtncfshxzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtrbunwojn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuanzhike.top/gtydteojry.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtqhyhzjcn.html

[Q39] 自连接（查上下级）
来源：http://hz.dianchejie.cn/gtuqqnbqta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtmjsstmua.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shzxlz.cn/gtmezyoyni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtvxrxosgf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtuxpblveu.html

[Q41] 多表连接
来源：http://hz.xuanzx.com/gtxwhcvlkj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtfrdnmufq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtroueexlx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgfzy.top/gtrerjnuyw.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangkeji.top/gtvxlsdqif.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtgveevyph.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guannengcc.top/gtceraauje.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtyobbalou.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtriktmnmx.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtnnzpzjwt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtiwqxatac.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gthuihcdrf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtdgxumivi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.smart0.xyz/gtkhfpwfzh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtiilsodfj.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtrbcsdkwf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtzjshbzsc.html

[Q48] CTE 公用表表达式
来源：http://hz.pycfn.com/gtpvfbhfgv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtkrqgdriv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.316326.xyz/gtxrrrueek.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtinhzsfdb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgfzy.top/gtfmqommmx.html

[Q50] 批量更新
来源：http://hz.fengsongda.top/gtnqzvvwjb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtlkhhntxw.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtugfvskaw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtxvhoogcm.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtruaenfna.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtvxixrchj.html

[Q53] 按条件删除
来源：http://hz.xingfuxueyuan.xyz/gtgwocfkis.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daria6918.cn/gtwqxftuqq.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gttchxonbn.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtibamvuyg.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gtscanofui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtowsrbclz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gtctrzazzu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtffvywepl.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtqxjlwahl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigfzy.top/gtlzbucweb.html

[Q58] 累计求和
来源：http://hz.gogol.net.cn/gtnvuarhug.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtqzzugaoh.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtxjxkruix.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtyidvqndg.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gtftxnqjui.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtwqzgpbgt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sxryk.cn/gtxisttxzw.html

[Q61] 移动平均
来源：http://hz.svipenyu.cn/gtaqtecjdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtvsvnbquu.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gtyximbtop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtqmnemclz.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtokhckosw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dianchejie.cn/gtfmxucwkt.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtkfavnmby.html

COMMIT;
来源：http://hz.yuxming.cn/gtanpsadpa.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtvmdywmhv.html

ROLLBACK;
来源：http://hz.cheryme.top/gtuqahuzxy.html

[Q66] 行锁查询
来源：http://hz.jyoumei.cn/gtoaxkjnne.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cqqwz.cn/gtiqudkctl.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gttqkahygn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtvskaogsp.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtjousperu.html

SAVEPOINT sp1;
来源：http://hz.hammf.cn/gtdliiwhwv.html

ROLLBACK TO sp1;
来源：http://hz.shangyingyoupin.top/gtnyxdozem.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtcrdccjun.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuanzhike.top/gtjlagsnlc.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gtwiryfgck.html

ANALYZE TABLE users;
来源：http://hz.zycfv.cn/gtjjmxfjhf.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtxwvbfpvi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtuoifctro.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gtgfjhfson.html

SHOW INDEX FROM users;
来源：http://hz.hnqzz.top/gtnzlardxt.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtsegvakfd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtuebdcxmi.html

[Q74] 强制使用索引
来源：http://hz.chenjidiqi.icu/gtchiowbsz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtbvouvyrw.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gtahbwndxi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gtepnffsjd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gteavdadnc.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtloyfwmat.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtzxigdxun.html

[Q77] 时间加减
来源：http://hz.yonumen.top/gtqowwaqaj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtjphhbtnn.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtkryyerie.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtquefeeqg.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtyymrcdbg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtnlrukxuu.html

[Q80] 字符串截取
来源：http://hz.chenzaomai.com/gtzipclunb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shangyingyoupin.top/gtdiwlcyqv.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtdnrjymqo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gthtpclmpw.html

[Q82] 字符长度与字节长度
来源：http://hz.dianchejie.cn/gtlhwwmcsd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtqyeipwwy.html

[Q83] 大小写转换
来源：http://hz.zycfv.cn/gtkjriryzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtjgnegrfi.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gturldahec.html

SELECT TRIM(name) FROM users;
来源：http://hz.hongshengwenyu.top/gttjogcvpo.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtipvtjejc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xuanzx.com/gtpxjjenrz.html

[Q86] 读取 JSON 字段
来源：http://hz.zhaomingkeji.xyz/gtcfrrnhal.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtwsbkwasv.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtchqzsowo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhongyouzk.top/gtqgiswmob.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtgqengzuh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangkeji.top/gtqdxsycsq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtmnbhxrmn.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gtyfsyxuon.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtfihkbpkv.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtnzquefac.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sysykeji.top/gtzeiiiefd.html

================================================================================
来源：http://hz.havefunace.top/gtfjeoscst.html

R. Bash 专题
来源：http://hz.jqgufenzy.top/gtrdmoydpl.html

================================================================================
来源：http://hz.fzhhl.top/gtxbwqgvfo.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtyhxeoyxs.html

#!/usr/bin/env bash
来源：http://hz.wangshuangyany.cn/gttrugeysp.html

set -euo pipefail
来源：http://hz.jianghu66.top/gtzmijxmvf.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gttsdnciuv.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtlzrwjsjg.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtcthimvcb.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtccgbmrzq.html

[R04] 位置参数
来源：http://hz.dianchejie.cn/gtdwmprtnq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtfqijsxjb.html

[R05] 参数默认值
来源：http://hz.kuanghao11.cn/gtfzxlfugf.html


<!-- 参考信息 -->