代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtuuprjyja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtzdiaewqs.html

[P03] 生成短随机字符串
来源：http://hz.c1oappe.top/gtyodvjrms.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtgncgwktt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.meibo888.top/gtkjwjoygu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtvacazzbs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtlbfwsygp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhixingplan.top/gtckciyvwa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtynpbwenz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guowangkeji.top/gtfwstifmn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gtrwtosqem.html

[P04] 求长度
来源：http://hz.sweek.top/gtyswckruf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtmwogrqfl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtuqvjsjdf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtgasrrpwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtueubzios.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cheryme.top/gtovwnjezz.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gttycyyslm.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtnbvaqmgu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenlongwang.top/gtwswglzve.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aibaodan.cn/gtpvidglxg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtclbneajr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtiyduatmu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gthqeqhpad.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gthopodcnj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gtsmonqjeb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gtkeqnahxy.html

Ruby: a == b
来源：http://hz.guowangkeji.top/gtvvazfezj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aizwys.cn/gtcxglvswc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtvaptufst.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtymtzxfcd.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gteeetgjnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtbanbimos.html

TS:   if (x == null) {}
来源：http://hz.xinyue.icu/gtwhwfduev.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtvndtrrrn.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtdvaxoddv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sweek.top/gtmklnzrfa.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtwabwbhzu.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtczibiwsg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.smart0.xyz/gtuewjwisj.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtpjoxonwc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtymwqnrqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtyvvxkdvr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtgbeyfjtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinyuanbaomall.cn/gtfqwgpnhv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhixingplan.top/gtqbrbwksd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fengsongda.top/gtkgudwuht.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtazwxdyzg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtcdkxtofj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtrdiiozwl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258888.top/gtnyaonsgd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtmzcpbdca.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jiagoushi.top/gtupkorstj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtnskcahfm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtzucfmywa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtwtaobfxa.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtiwgjuiwz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtzakxaufd.html

================================================================================
来源：http://hz.fengsongda.top/gtogfzzlju.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gthwistwms.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtazvsqdda.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtrdfkkvww.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtknpxldgl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtfvenacnf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinghuilouyu.cn/gtidjnzsqy.html

);
来源：http://hz.jlsjyb.cn/gtzzimssdz.html

[Q02] 创建带外键的表
来源：http://hz.9152youxi.cn/gtfnhsuohi.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtjipohxas.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtqvckwkvb.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gtygilxmdd.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtcwokjmgd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtxvauiuyn.html

);
来源：http://hz.zhijiandao.cn/gtltjdtifh.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtxwexzqzy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zycfv.cn/gtqxftmfsv.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtrqnvucqy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtxqmdoepu.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtvpntqxlf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtqbjfvnjk.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtxbgxdhva.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tanke756.top/gtsisqdzmq.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtkmvuvled.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shangyingyoupin.top/gtqdgtrmtm.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtujgxmmhf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtzmkwunsd.html

[Q09] 创建唯一索引
来源：http://hz.yangfankeji.com/gtxwsudbfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj202588.top/gtnvucarxj.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtmbnfgsgb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnxiangtu.top/gtqqbwmeds.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtttvlknue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtjztrfnps.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gtqjsgxskm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hfpthk.cn/gtsmcqmlxm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtpstfhpzg.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtrcchprxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gtfsjnjzbm.html

[Q14] 存在则更新（upsert）
来源：http://hz.sysykeji.top/gtuisvnisg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.9152youxi.cn/gtuxzlhzsy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sufxvd.cn/gtcplhgpxy.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtbtanuyfe.html

SELECT * FROM users;
来源：http://hz.nwbrower.top/gtlurrguvh.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtjbmdyntp.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtyrtjgmbh.html

[Q17] 条件查询
来源：http://hz.chenlongwang.top/gtrudxckpx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dashuyun.cn/gtklvxzhza.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gthtohiodf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtbsbhueui.html

[Q19] 范围查询
来源：http://hz.zhixingplan.top/gtoassyqes.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtokdjndax.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtrcdoxvxe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtunfsfhxu.html

[Q21] 空值判断
来源：http://hz.meibo888.top/gttwnzkqoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtknaspptm.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtuelubpvu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtzuxdowbf.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtilfhjqep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtjgfenwri.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtvsmxxgng.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtwvfseluv.html

[Q25] 只取前 N 条
来源：http://hz.havefunace.top/gtenjrxydn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtgrqifvhc.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtbdlwlmmk.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtyyocdclk.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtskrymwkn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtugfbbeob.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtxlfxrurq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtqkpnhkhf.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gttiwepyyo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gthqwgztzc.html

[Q30] 分组统计
来源：http://hz.xziqi.cn/gtpzrrvvne.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtiwdjkqcr.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtoijuitfv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtxaywxccg.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtrwzcjfgd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtjfkumydv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtgwvkzqci.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtljmizury.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtdqldjyai.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gtgvydbigq.html

SELECT * FROM (
来源：http://hz.cheryme.top/gtycmyzdkb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.vqdsnc.cn/gttrcovvoc.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtkcfesdps.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtoslgjiln.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtabsxxust.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtnnizvaou.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gttvwsxsal.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtwvopezkf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gtzyjkezfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxuanxn.top/gtvtgofjbb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtoixltlxt.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangkeji.top/gtmrnhgwhe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.birdmap.top/gtszabyjxn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtzpozptrf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigfzy.top/gtfoephbrh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.havefunace.top/gtzaanizgo.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtxrgvhtpx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtliemqnxm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtbvaygnwv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cucudq.cn/gtwwvnxzsc.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtkhwuuvqb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtdnovlkjx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtivqtzuba.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtiifgfitv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtwhzorath.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtiskifxuh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtshrdsamc.html

[Q45] EXISTS 判断存在
来源：http://hz.zdqjudy.top/gtlwnxzglw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtfdislxib.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gtuzoenlkz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtisuzmotk.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gtbcnmzxis.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zycfv.cn/gtopwwyvzn.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gtejkqqenl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtzakzayib.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtyszgdtim.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtwcifpncx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ivvv.top/gtgaefusym.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtqeardwac.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtrnbhkngo.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtettlilqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydjk.org.cn/gttdpynvhj.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtssgfcfvf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtlyyjnynf.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtbgdkvxhd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.redwolf501.top/gtakvutucp.html

[Q54] 清空表
来源：http://hz.gzhubu.top/gtnrdgkngj.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtquromwkp.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gthmawxxmo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtcqfirbir.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtdwdsfelj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gthoktbeoa.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtezcnjolu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtlbdbzizl.html

[Q58] 累计求和
来源：http://hz.tianlin.xyz/gtmpotfmoh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhixingplan.top/gtzsjtwipq.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtjtlsukmy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtjxnjlevx.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gthwcyofti.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtifxywgcf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtzzdmxzpi.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtkevpgyve.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtbfdpiceo.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtigriibvn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gthaxnuxge.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtosmsueba.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dianchejie.cn/gtwqtjsxnk.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtfvvoyyht.html

COMMIT;
来源：http://hz.ybcxt.top/gtadkhihzm.html

[Q65] 回滚事务
来源：http://hz.tianlin.xyz/gtzaiidprk.html

ROLLBACK;
来源：http://hz.ybcxt.top/gtxyrjevzz.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtlvsiesvs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtghuvcglm.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtamtdqydi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtgfakwvha.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtsqrfhplb.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtypjmhdbz.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtzjxhysak.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtbtgbqaht.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtbshjelbh.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gtxpqgkgix.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtekiaxguo.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtjjoygehy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gttcfztbvy.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtsxbtuiyj.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtfbchobmn.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtgbdtioca.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtqtxiiprd.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtkfxkrugt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtiecfmfrr.html

[Q75] 日期格式化
来源：http://hz.guowangkeji.top/gttukagpcc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtcceszavu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtcqtobwip.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtbrljonvf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gtzriqpjwj.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtgeqknxob.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtxqgfayhw.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtbcnytlwt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtfgxludlv.html

[Q79] 字符串拼接
来源：http://hz.gogol.net.cn/gttcqrfjdj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gteuioeunt.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtfaxfxmeb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtscvatzxy.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtpkifhnol.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtmxutlcoa.html

[Q82] 字符长度与字节长度
来源：http://hz.gotoacloud.top/gtwdsfrhwv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gtxkmbvlbe.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtdpxtwnmp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtlnvrxwxj.html

[Q84] 去除首尾空格
来源：http://hz.cqqwz.cn/gtqroiuknt.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtihkmfzkt.html

[Q85] 数值取整
来源：http://hz.aizwys.cn/gtsepimpwf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtjprtjflb.html

[Q86] 读取 JSON 字段
来源：http://hz.tian-w.cn/gtenkcjvci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangshuangyany.cn/gthwycmtmv.html

[Q87] JSON 字段做条件
来源：http://hz.meibo888.top/gtnavtnekl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtqsaaxlkk.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtepaclbgm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtrdghrwlf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtcrbnwwmv.html

[Q89] 判断表是否存在
来源：http://hz.jlsjyb.cn/gtltwrtpin.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtfzdolrhr.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtfiknvsdv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gttdjfouzr.html

================================================================================
来源：http://hz.gogol.net.cn/gtiuymnrlg.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtiyrkqprk.html

================================================================================
来源：http://hz.jianghu66.top/gtbsbzovve.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtsbprwtaz.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtnryozkds.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtlodpxakk.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtpoyaxukf.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtxdwuhsbe.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtsfiyqxbg.html

readonly PI=3.14
来源：http://hz.hnqzz.top/gtgqogedgb.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtrkykkyqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtntwlwxvf.html

[R05] 参数默认值
来源：http://hz.cucudq.cn/gtvqxvyxeb.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtombxmzvl.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtdbzgatgv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtcgxiuyfr.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gthngbxhuy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtjpcnsusl.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtgnkacdwe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gtjdovoila.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtyvecnlpw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtycmykjug.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gthvdzhlrk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yongpay.top/gtcgqyflxk.html

[R11] case 多分支
来源：http://hz.nanxuanxn.top/gteffxzjdp.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtbmgxruzm.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gtplcnifmh.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtqwhpturj.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtwjdfvgmp.html

esac
来源：http://hz.c1oappe.top/gtwvaijlyu.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtfrotrrko.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sxryk.cn/gtxbzdulzm.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtfkdmzogc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtxtehcrff.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtukgdnpit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gttkbyvvji.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gttiebhzqu.html


<!-- 参考信息 -->