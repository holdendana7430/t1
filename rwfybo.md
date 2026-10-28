代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtkgjuakab.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinyuanbaomall.cn/gtspowtwxt.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtfrnjzqja.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtluhzjidz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.smart0.xyz/gtxdmvidmt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtqvshqefr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtckyxztsd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtqpyxvmdm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jyoumei.cn/gtxjcjemxz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cqqwz.cn/gtgrncccpn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gtyhbyjlju.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtvpcqbzqj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gtetyeylki.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtvffqlccd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtqvioolyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtcysbtwlz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtegmlaqbr.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gtoxsmpstb.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtyksofihh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daxiang520.top/gtiqejpree.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zdqjudy.top/gtjqzcqgze.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtilspkqeq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtgtrcvsoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gtdvrpoyjh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtsmqehbfj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtggwstapx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtzocpmaly.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtayotjrcg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtaxhabqku.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtaqpskhvf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shanyushiyangtech.top/gtphzldpur.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gtzuzhllbq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fengsongda.top/gtdqncssxb.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtbwzmmawy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtfjelodac.html

Go:   if x == nil {}
来源：http://hz.jianghu66.top/gtrlsmvtwn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtfrcufwae.html

C#:   if (x is null) {}
来源：http://hz.hongshengwenyu.top/gtokxkxrec.html

[P07] 防抖与节流
来源：http://hz.yj202588.top/gtyzkbofyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cucudq.cn/gtnovpmxwk.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxinkj.top/gtinqyfhwl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtdemcnigx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtvxguhcnd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daria6918.cn/gthkngegve.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hongshengwenyu.top/gtgokkaedj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gtzthtutxl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gtzewbgdpq.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigfzy.top/gtpearczgf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtxjhxjzgy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtiitccqvu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cashguo.top/gtvtumzoop.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtymfcgqxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtraqvlmmz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.iojbl.cn/gtbnhfluqh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtxczbdqne.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guowangkeji.top/gtqhvycizs.html

================================================================================
来源：http://hz.yueranfly.top/gtolixjcke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yueranfly.top/gtlpkbpzcl.html

================================================================================
来源：http://hz.andypj.xyz/gtfbdddzoy.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gteskcdmhn.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtklctbfbs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtywywvrfb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtpnpzxuyk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtnbduuwlb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtcbppztng.html

);
来源：http://hz.xuetiantiany.cn/gtfsmkypqy.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gttlnyaesj.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtiphhlfld.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtuaetibap.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtmmaewpml.html

amount DECIMAL(10, 2),
来源：http://hz.ydzc1.top/gtibmuinty.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ybcxt.top/gtzcrvvcnd.html

);
来源：http://hz.hongshengwenyu.top/gtraqzcmoi.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtnylcdlgl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtcszqzlnb.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtusmdfott.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtwwznciwr.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtrfnjiyww.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtmapnxeuf.html

[Q06] 删除列
来源：http://hz.zhixingplan.top/gtvhoxzzds.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtenirjdot.html

[Q07] 删除表
来源：http://hz.yanxiufei.cn/gtrwbcclox.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtdyokllun.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtfcuwosxu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtlqcojxry.html

[Q09] 创建唯一索引
来源：http://hz.jinghuilouyu.cn/gtubmbssug.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtvdiqvcig.html

[Q10] 插入单行
来源：http://hz.feifeiyinyue.top/gtbutudfxo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtiamamxpp.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gtqxbvwuoq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgfzy.top/gtwqzoexwj.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtmhprveny.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtemchokic.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sxryk.cn/gtlismsojl.html

[Q13] 忽略重复插入
来源：http://hz.ehwqpu.com/gtxkuoomkw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhixingplan.top/gtagxoagan.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtuzmfhqer.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ywan-chungtsiang.top/gtfndbbxpr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtkhfrnduu.html

[Q15] 查询全部
来源：http://hz.shanyushiyangkeji.top/gtarusolax.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtaflpgved.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtqbocpphf.html

SELECT id, name FROM users;
来源：http://hz.havefunace.top/gtpijreill.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtivmvorny.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtiqyuppbt.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtoooliolt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtardierdg.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gtidmracur.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtgwewtkyl.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtdsoaooda.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtpwcnqagi.html

[Q21] 空值判断
来源：http://hz.gotoacloud.top/gtijsjzimx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtuqxwxmxw.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtlhpkwkkv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtnoghmmzj.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtlxepxlcp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtojrohjkt.html

[Q24] 去重
来源：http://hz.xuanzx.com/gteiabodft.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gtcypbnxtu.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtmvuhtgdj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhongyouzk.top/gtncasfstk.html

[Q26] 计数
来源：http://hz.ppjwa.cn/gtygfwsrsi.html

SELECT COUNT(*) FROM users;
来源：http://hz.jlsjyb.cn/gthmvpigpk.html

[Q27] 条件计数
来源：http://hz.zhengqikj.top/gtorjcovcn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtslrlhpaf.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gthnbdntme.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtlkoemxdc.html

[Q29] 最大最小值
来源：http://hz.jinyuanbaomall.cn/gtjsikfrrk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cucudq.cn/gtslgbspdb.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtrostmanq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtpshngbce.html

[Q31] 分组后过滤
来源：http://hz.52xcode.cn/gtqimqubbb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtrjqlpboj.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtucvkmhsd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtiwzrlkll.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xingfuxueyuan.xyz/gtzedhrtfg.html

[Q33] 多列分组
来源：http://hz.havefunace.top/gtrlxemrix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtzpmlwsfz.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtywpobwci.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtxzvwcvqz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtpfftmrlm.html

) t WHERE rn = 1;
来源：http://hz.gogol.net.cn/gtiidgkhgr.html

[Q35] 内连接
来源：http://hz.zdqjudy.top/gtmzxtqgfi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtvzhgtavx.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtnztyuhlf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtsteejhpq.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gthehisfmn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gtooboeeey.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gttjbjumle.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtqgyxthlj.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gtujxrcula.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtzsvhbwpk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtwudtnacv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fengsongda.top/gtvchkhxbb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtqtwutsus.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gthlbpuudb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gtautzlwiz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.c1oappe.top/gtgunhlcuq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtamgsrorc.html

[Q42] 连接条件附加过滤
来源：http://hz.yj202588.top/gtdcgqedmx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtdndakqmd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhoulong.xyz/gtftuimurp.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gtcanankpb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtwbgstxnq.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtlnnccakq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yanxiufei.cn/gtgvrgbmhp.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtdwzeiraz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtjdbnxcvz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtjcyabntc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtetjakedt.html

[Q47] 与平均值比较
来源：http://hz.cheryme.top/gtqrquwedq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fengsongda.top/gtcxrlzbyq.html

[Q48] CTE 公用表表达式
来源：http://hz.xziqi.cn/gtrkvdpcry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtqsdthutg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtiijdmyyf.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtzkalxnit.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtjlmqyxjo.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtmfdyfgcp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtvxcmnoqr.html

[Q51] 用子查询更新
来源：http://hz.hammf.cn/gtefwdhmqb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtvfmsyxcu.html

[Q52] 删除指定行
来源：http://hz.ydzc1.top/gtohfqghet.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gotoacloud.top/gtyvbtamvp.html

[Q53] 按条件删除
来源：http://hz.jinqigufen.top/gtfijsjytm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtyrmaeuws.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtvekiiswu.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gttlgexqgk.html

[Q55] 排名（并列占位）
来源：http://hz.tian-w.cn/gtbtpjyjdd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtxsfvxfvf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gtxbkwftzg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.kuanghao11.cn/gteyfgbhnd.html

[Q57] 行号
来源：http://hz.zycfv.cn/gtdtoolbcc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtklatqeqe.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gttzakhbxg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258888.top/gtdaiqomez.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gtjmbvannb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtkolwgsub.html

[Q60] 取上一行 / 下一行
来源：http://hz.xylfe.cn/gtgyjfagll.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtocgctfrj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhengqikj.top/gtbboosyvj.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtcqhypgnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtlfbbszjf.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtuywqwsqh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtcsnchhlm.html

[Q63] 开启事务
来源：http://hz.jlsjyb.cn/gtbocptota.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.svipenyu.cn/gthqecboxy.html

[Q64] 提交事务
来源：http://hz.hnxiangtu.top/gtmutfznke.html

COMMIT;
来源：http://hz.fengsongda.top/gtnellemqm.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtgeomgmxl.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gtvedozvzx.html

[Q66] 行锁查询
来源：http://hz.hysaishi.cn/gtiikmelzd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtmfyjtcng.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gtjjoettcf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtmbknsfra.html

[Q68] 保存点
来源：http://hz.meibo888.top/gtzcjfehgz.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtxvvtthft.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtlflomfgs.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtkuninppl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gttpwchhlw.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtwnoqiwxp.html

ANALYZE TABLE users;
来源：http://hz.yonumen.top/gtgamfmiol.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtwyawgsta.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtnijeloir.html

[Q72] 查看索引
来源：http://hz.kuanghao11.cn/gtdnbnngzc.html

SHOW INDEX FROM users;
来源：http://hz.hammf.cn/gtculwdkwn.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtpkoclykv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtkhovjati.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gtxeqvjodm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gtvjrprbir.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtpvmnbbdi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gteoujaelb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtetzfcejj.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtagsafmfi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fzhhl.top/gtikzxhxzj.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtcapuupoi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenzaomai.com/gtvfukmuuo.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gtzupmrqbs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtujlvzjri.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtbcoieyym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtmvhtzsjn.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtpkobfuek.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhoulong.xyz/gtnhnlycer.html

[Q81] 字符串替换
来源：http://hz.birdmap.top/gtwyuityba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtmpdlqbdw.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtlgxrretr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtdyazllqp.html

[Q83] 大小写转换
来源：http://hz.zhongyouzk.top/gtzntwfuwz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pycfn.com/gtyjrunrtg.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtezsdswbl.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtflmwgayv.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gtsxifwlgs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtpawspedt.html

[Q86] 读取 JSON 字段
来源：http://hz.zhoulong.xyz/gtvvlgmdya.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtrfcciljv.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtmogllvkq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.svipenyu.cn/gtgwwrdnbr.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenlongwang.top/gtwlmwgzop.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtsabhsyhq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtmrqrumje.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtmsvorxxi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhongyouzk.top/gtgusmriyy.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtzjlxgnmm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gttcegiogg.html

================================================================================
来源：http://hz.ppjwa.cn/gtkyqsqzcr.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtwjknhwyp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbnuxihhw.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtyomuodfg.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtklddqdnz.html

set -euo pipefail
来源：http://hz.yueranfly.top/gtmkoztxxg.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtknolulqn.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtuvmocgqw.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtwrezregr.html

readonly PI=3.14
来源：http://hz.yuxming.cn/gtozxmputx.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtltpbchvl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtqvuvwmec.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtgbktwwxq.html

name="${1:-default}"
来源：http://hz.ywan-chungtsiang.top/gtccyygnev.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtctbeoqlj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtfbodhkah.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gthyvpodrx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtunkhfmtm.html

[R08] 数值比较
来源：http://hz.guannengcc.top/gtiibuaiqc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hongshengwenyu.top/gtfdenvaeg.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtatteiszk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dashuyun.cn/gtgtoipvnc.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtmykihugs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gtujaqmqex.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtxocxamcy.html

case "$1" in
来源：http://hz.tianlin.xyz/gtmuzldcuj.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtwewcknxm.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtgxlagdme.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gtomaoddsq.html

esac
来源：http://hz.fzhhl.top/gtdaodgycw.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtawehcbca.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtihhibypb.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtduyosvbt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nwbrower.top/gtgiawyaoc.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtbxihvfnl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtcbewpdal.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtcvrhsmex.html


<!-- 参考信息 -->