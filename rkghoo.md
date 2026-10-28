代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtrtqyqnto.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtzbdofolw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhiwuduotai.top/gtrnhxfjyy.html

Ruby: SecureRandom.uuid
来源：http://hz.hfpthk.cn/gtrnlhajmq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yueranfly.top/gtoiiejcfh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtyflkyjte.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtoydshkjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtphccqvdt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtehgigvva.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.snrcjt.cn/gtklsnlzyo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtfpzbndev.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtahyubvdw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hammf.cn/gtjhzsdmog.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gtemrgmtlu.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtudfwpbun.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtjljsvuwj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xinyue.icu/gtdhuptmpm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtjyzjldne.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtdljkctuh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gtdssdencu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gtagptmnnl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtzdfjcnom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gtiqnddrjk.html

[P04] 求长度
来源：http://hz.dianchejie.cn/gtuevaeqao.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtphpqgara.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtzhsnqhmb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtqwrgtmcw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtcnntjbek.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtvczvmexf.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtfyaktfss.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtnwlbtnus.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtzmnhfext.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xylfe.cn/gtislanixz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ivvv.top/gtzoieokym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtfdoglhxg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.9152youxi.cn/gtqxgdvstk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtyqcesqrh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydjk.org.cn/gtgtphyogv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtekxhxmid.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtgypvbjbd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxinkj.top/gtsdlkfavi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuxming.cn/gtxxnyhecl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtkqbhvqtd.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtyeskmhao.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.9152youxi.cn/gtohxozcsd.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtlnukadfe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtaibsfzlo.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtjjwutjaa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtloltesyl.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtgjuysvsu.html

[P07] 防抖与节流
来源：http://hz.shangyingyoupin.top/gtmcagyiij.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtjjluztri.html

PHP:  // 手写时间戳比较
来源：http://hz.hongshengwenyu.top/gtgirbilbe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtqdgvuewp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtbnoabmra.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtvbaxoion.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtoeplqnmz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gthzqidoto.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhijiandao.cn/gtuecgotnq.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gthnggjasj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtnlgclcxe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gtppkzhhup.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtenldgfbx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtuaazjuau.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtswwpnqvq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtftlxdzpi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtyarrisch.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtstypostn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkblqtufz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gogol.net.cn/gtzhchfmrc.html

================================================================================
来源：http://hz.316326.xyz/gtbvpbzxfu.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtyzvnvncv.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtdcsrfzdr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtpnanpniz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtjqexbver.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gtaynpxmqy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gthikduayu.html

);
来源：http://hz.zycfv.cn/gtlwdzeecz.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtdicgvzvd.html

CREATE TABLE orders (
来源：http://hz.yuanzhike.top/gtmmttstgh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtbdsxmfoz.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gthdklwcwy.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gthvhxxwpq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gteirgjsty.html

);
来源：http://hz.yj202588.top/gthndcdcsu.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtaylwepyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zdqjudy.top/gtwxixzpad.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtbgqbpudq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ydjk.org.cn/gtehcarsna.html

[Q05] 重命名列
来源：http://hz.cucudq.cn/gtcgiicufx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtuarzxrxc.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtzjcyvnhz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtlxfkvcup.html

[Q07] 删除表
来源：http://hz.hongshengwenyu.top/gtxhpfucnl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtjpbmninm.html

[Q08] 创建普通索引
来源：http://hz.guowangkeji.top/gtrszkblzo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtonzlkpob.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtxslogtxa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtnkwlmdjv.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gttzytfyrc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gtrkboayfl.html

[Q11] 一次插入多行
来源：http://hz.jqgfzy.top/gtcrjuoiuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtolagcgfp.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtcekmsnif.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yanxiufei.cn/gtitdeapnu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtzvtgrvdr.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtlsqfvzon.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuanzx.com/gtywjhbeuq.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtriiwfktf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gtiunvnink.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.snrcjt.cn/gtfzuooadk.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtivsegnbq.html

SELECT * FROM users;
来源：http://hz.yongpay.top/gtvgwgzovm.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtdcbtptrk.html

SELECT id, name FROM users;
来源：http://hz.guannengcc.top/gtkkrnxujq.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtozhcjzgx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtprcvrsoh.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtisyfjfcn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtigjeukys.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gtfnyfwdzp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtetlixhsn.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gtcbzrwhyc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangtech.top/gtvbgtontt.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtomdmxmwq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgfzy.top/gtfihxkupc.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtyenlozow.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gtoyshdyza.html

[Q23] 分页
来源：http://hz.tanke756.top/gtfzyxmhfb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtgndjdboc.html

[Q24] 去重
来源：http://hz.chenlongwang.top/gttycnmxsd.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtdsqxqrhb.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtrswrkusd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtmicnnmbd.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtgfnioezz.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtfgqmcyre.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gttetlfgra.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gttrtmpdnw.html

[Q28] 求和与平均
来源：http://hz.jqgufenzy.top/gtltijaunf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtjwxtwwys.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtfwcxzllu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtbhkmrons.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtdvlexfip.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtafenndhw.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtqglwhrxc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jiagoushi.top/gthntnydac.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtqrwwaahv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtzlwgkixl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtjzdukmfv.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtmvhrhdnn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhijiandao.cn/gtvcreaupi.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtsuexcfei.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtfrbgifyq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuanzx.com/gthrpnkohs.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtgzkqxxjj.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtovvbofou.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtzqpdecsh.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gthqamndbn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtniuiaqhv.html

[Q37] 右连接
来源：http://hz.aibaodan.cn/gtqzpbkmpp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gogol.net.cn/gtkzvvdijv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gthberlrob.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtsrnilqwt.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtnnvyyjmt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gaohongyu789.top/gtafazfxht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtdfbaiiap.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtckmojlbj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtorkyvbyv.html

[Q41] 多表连接
来源：http://hz.pycfn.com/gtzztsmjsy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtpdarqrwr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtrkkvqjgk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtiigbhgct.html

[Q42] 连接条件附加过滤
来源：http://hz.yj202588.top/gtjrozigxj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtyhgvfuih.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydzc1.top/gtvgopwuqe.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtlritzgem.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtcjpecvsd.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtvampohqh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zdqjudy.top/gtgnfbicib.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtrokobbgi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtppeffdta.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnqzz.top/gtskawgrnw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtkdoqgfkq.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtcubpgyhn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtlmfiwtvj.html

[Q48] CTE 公用表表达式
来源：http://hz.chenzaomai.com/gtiyzzhymg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtvdfbsbxa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtiesageqy.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtqosflqqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tanke756.top/gtcqqahidj.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtgdrhzkea.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yonumen.top/gtormgboqm.html

[Q51] 用子查询更新
来源：http://hz.jqgufenzy.top/gtbdhecpfs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jlsjyb.cn/gtrcqtmzth.html

[Q52] 删除指定行
来源：http://hz.yj202588.top/gtkmdpdvol.html

DELETE FROM users WHERE id = 10;
来源：http://hz.0kj1m.cn/gtxqjtupzt.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtctmmljfr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtireuidlz.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtbhozrvpy.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtmhnriayg.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtfjkdyofe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtowhisuuj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtkirgyvaj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gotoacloud.top/gthczbdoqu.html

[Q57] 行号
来源：http://hz.pycfn.com/gtkmthmtjj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtjjvxstjz.html

[Q58] 累计求和
来源：http://hz.cucudq.cn/gtuzahdrtt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gthjkzcbnd.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtdarsjbat.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenlongwang.top/gtwagcnhoq.html

[Q60] 取上一行 / 下一行
来源：http://hz.dashuyun.cn/gtpeeonljx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtpszcgxur.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtjtubkyfd.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtgytchvnd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnxiangtu.top/gtlthawmwo.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtplyddmom.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gttoceauuz.html

[Q63] 开启事务
来源：http://hz.xingfuxueyuan.xyz/gtbwgtzoud.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258888.top/gtsyhubcre.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gtwcsulsql.html

COMMIT;
来源：http://hz.shuidangran.top/gtaaqjuqnn.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtryuoypjf.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtaqxnxofm.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gttrtksbue.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtttsgpods.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gtbzoclhjk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtygpdrlud.html

[Q68] 保存点
来源：http://hz.vqdsnc.cn/gtwjtwosok.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtdmzjklgn.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtqhzcjgla.html

[Q69] 查看执行计划
来源：http://hz.guannengcc.top/gtmznbuufw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gthyzejsbb.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gtpkwcdpox.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtzdbucyxl.html

[Q71] 查看建表语句
来源：http://hz.jinqigfzy.top/gtplkkhnux.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.bjfxy.top/gtiescmkvf.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtemgekbyz.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtbjuaehih.html

[Q73] 查看表状态
来源：http://hz.nanxinkj.top/gtnmhofagh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gtlpmlvmwq.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtnjsazawk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtdfyowcfl.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtmtkvbjct.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtlgcohqyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fengsongda.top/gtcdvaesyi.html

[Q76] 按天统计
来源：http://hz.52xcode.cn/gtsjfmvvcp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtekaolwjj.html

[Q77] 时间加减
来源：http://hz.vqdsnc.cn/gtgeobtzil.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtlheootmb.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtxetiidqy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtxryikgfb.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtykwrkhic.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tian-w.cn/gtvbwxbjib.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtzamsbllz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gthnciwbtz.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtjcknfkgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gtfhrmkaaa.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gttghlgojv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtadwetdie.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtcwyaleld.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zycfv.cn/gtwipoiros.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtbmdnyiry.html

SELECT TRIM(name) FROM users;
来源：http://hz.aibaodan.cn/gtqdcvaqkb.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtrydtcnqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtyvpophik.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gtoqnqcplt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtuyjqlilx.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtogekbusz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cqqwz.cn/gtylauwivq.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenjidiqi.icu/gtjhdjbqyj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gotoacloud.top/gtgpkkvuje.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gttefkomci.html

[Q89] 判断表是否存在
来源：http://hz.yongpay.top/gtigyteerz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sxryk.cn/gtabxqmhnq.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gttxewoyka.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtoyjzxvhe.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtobfkenpk.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtbqkymbyx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjrifyvhs.html

[R01] shebang 与严格模式
来源：http://hz.nanxuanxn.top/gtetvvebbo.html

#!/usr/bin/env bash
来源：http://hz.hnqzz.top/gtxaxqvkhl.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtqroizlzq.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtpcnwhihj.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtxkqitqvz.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtdcvosnbn.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gthrlhvmys.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtecpofypn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtshagjewg.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtmlocatlz.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtiwnrrigm.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtxpqqnbct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gtdtyadgjs.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtmmncxiqq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtwrvzchnf.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtdupgywns.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtkcezmwgg.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtzavlpjjq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtwsyjsnem.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtxmfauuqo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtdimrcjde.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtebymvweh.html


<!-- 参考信息 -->