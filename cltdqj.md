代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtmngfvjka.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtfmvbddzg.html

[P03] 生成短随机字符串
来源：http://hz.aibaodan.cn/gtnviruttx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtvonxxoou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtuelcuozm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gteyhryjdu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtptxnmgvz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gtwwhlbrrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinghuilouyu.cn/gtaflqxuvy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtelcsoquy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtjhbnksqa.html

[P04] 求长度
来源：http://hz.guannengcc.top/gtdcvomfoe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtxyexqmnh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtsshexylw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtegnsbxpp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtdgezxzxv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtjpfwsgpm.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtkwvohxxu.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gthixicwxw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtgnhxypuc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shuidangran.top/gthpxluyrs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenlongwang.top/gtpezstyvv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtconmwajp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jiagoushi.top/gtiwhmdtfx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtsadzyemj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtljjlcetm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtmrurvnfy.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtzhaphejn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jiagoushi.top/gterqaneoi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtrpetyaar.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gthyhcisal.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtdustwbdf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtumwoyzoe.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtslxrrvcs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangtech.top/gtxkugvwye.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtrwonkswy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tanke756.top/gtqlrbgemc.html

C#:   if (x is null) {}
来源：http://hz.yuxming.cn/gticfcusbp.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gteqaazlrn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtqpczuumt.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtocepxegq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtssdywaot.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtevbijfyo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtiyxmglkg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtglpadacr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtrclhpdkm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gtqfnhzjav.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtbjbmzlvy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtwqizqxie.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtlmhugvyl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gtwsnwvlii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gtyyacigho.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gtidkplont.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ywan-chungtsiang.top/gtoooqstti.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gtlncrtlbb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tanke756.top/gtsbomkctm.html

================================================================================
来源：http://hz.nanxinkj.top/gtmqzfiyua.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gtovaechlp.html

================================================================================
来源：http://hz.chenlongwang.top/gtznfzzbvt.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtptyqggvt.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtfzpiiufg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtmztlifsi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtfinyyyyk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shzxlz.cn/gtoiucjrno.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtvztvazul.html

);
来源：http://hz.gaohongyu789.top/gtcvuthibb.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gtlkgiwofb.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtwspsxyuv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtfndflqet.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gthnwiwxrz.html

amount DECIMAL(10, 2),
来源：http://hz.fzhhl.top/gtmhrrltcz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhijiandao.cn/gtmvxaswqp.html

);
来源：http://hz.zhoulong.xyz/gtvjehhkvg.html

[Q03] 增加列
来源：http://hz.zhaomingkeji.xyz/gtvgvcnflq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtzxfxvbpo.html

[Q04] 修改列类型
来源：http://hz.kuanghao11.cn/gtymzbffwu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tianlin.xyz/gtcvcknfaj.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gttvolrscf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.bjfxy.top/gtnibwpsrr.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtclcornfh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gthpqzrlwq.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtdvrmjgwe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtyulhxocx.html

[Q08] 创建普通索引
来源：http://hz.pengpengdd.cyou/gthebjzznn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gtbctjuweo.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtlgfjlvdt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtfwmrwphr.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtyhbnknad.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gthpodwvey.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtjhxhlejz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gthsjdrtzq.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtpwsfrazo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtrgtnrdtk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cucudq.cn/gtlyfiaops.html

[Q13] 忽略重复插入
来源：http://hz.ydjk.org.cn/gtrblyznjv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtypollprb.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtuldlgxac.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gthegleofm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtqpoiuzje.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtukxdqkcz.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtpbfnhqzx.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangtech.top/gtzgcruqay.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtetquoiuo.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gtkiqvfuxy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aizwys.cn/gtxswlpbde.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtesfgniih.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtpnqjwceb.html

[Q19] 范围查询
来源：http://hz.ydzc1.top/gtjrceudyq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtrlnfuoud.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtvsmgxjhv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangkeji.top/gtviwzadsx.html

[Q21] 空值判断
来源：http://hz.kuanghao11.cn/gtrlpdkcax.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gtmemmbass.html

[Q22] 排序
来源：http://hz.tanke756.top/gtuvumdkvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gtnigwfykc.html

[Q23] 分页
来源：http://hz.yuxming.cn/gtdesdsjbb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gtkaahnzmq.html

[Q24] 去重
来源：http://hz.ydjk.org.cn/gtjjffsfpi.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtryuxloek.html

[Q25] 只取前 N 条
来源：http://hz.9152youxi.cn/gtluktujym.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtrvbnrtnz.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtnbntgrmg.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinghuilouyu.cn/gtemhymerd.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gtdvyhkkcw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydzc1.top/gtqkighjby.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtmizvjcyf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hongshengwenyu.top/gtfrzdlcdx.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtsojkzuar.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtmvjdixxf.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtkzxlsiuq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtyaegrqjy.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtlpzaixre.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtykupeqtp.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtouoqhxod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtegtynviz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xingfuxueyuan.xyz/gtonxayckx.html

[Q33] 多列分组
来源：http://hz.redwolf501.top/gtbffwjnks.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtqayxuhzd.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtycmyqqri.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtqdkgvtyw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guowangkeji.top/gtcilzisza.html

) t WHERE rn = 1;
来源：http://hz.svipenyu.cn/gtyhrpmegi.html

[Q35] 内连接
来源：http://hz.shzxlz.cn/gtbnnsyrrw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtldwbtnzc.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gteqcndbkp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtkwrhfchl.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gthjsrtyia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtiyjngrcm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangkeji.top/gtbwmpbwoi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtpheaauam.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtalkvmmty.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gteeuiddnr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nwbrower.top/gtishmhwfl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtobsklamm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dianchejie.cn/gtvozqixhb.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtlbplhcrs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtdsrwxnun.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gtnqjwqbyd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenlongwang.top/gtvsyvcywg.html

[Q42] 连接条件附加过滤
来源：http://hz.sweek.top/gtissumifx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtwfywbczo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhijiandao.cn/gtfuvmfegs.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gteophryjn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtuctiyyxr.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtecpelhog.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gtgugoapye.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtuliwbqye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtyfppumfe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtqqcwmgoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtjhitevjt.html

[Q47] 与平均值比较
来源：http://hz.xziqi.cn/gtojhsrzga.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtaunnvcxm.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtjhiwkyzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtvpmlrsdi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtdrneydol.html

[Q49] 更新单行
来源：http://hz.mhx1999.top/gtqtpxtzhv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtqbpzgxtb.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtqndtjefl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenlongwang.top/gtzquxdpmg.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtyhshqxlv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gthancejcj.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtbhmtbzwz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gtcqpltsvq.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtukesrxyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zdqjudy.top/gtieysbubi.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gtjdloxske.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtwklliple.html

[Q55] 排名（并列占位）
来源：http://hz.smart0.xyz/gtcdmmxkrh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtjhanljyd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gthyitpkcp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gteyhyzfhv.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtlxjnqwer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtddkvrxop.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtbhxyeadz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gthxrdunli.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gtsmbwbxzq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xinyue.icu/gtxlbpuzed.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtlkydnigc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtljtobbvc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtadqxjsaw.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gthqykntfg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtrjiiwmgt.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtbqtnsmjn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtcldbbzgm.html

[Q63] 开启事务
来源：http://hz.andypj.xyz/gtzyqvyuhe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtgnocorzj.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gthoccgvfh.html

COMMIT;
来源：http://hz.zhixingplan.top/gtdtzxiocg.html

[Q65] 回滚事务
来源：http://hz.gotoacloud.top/gtegasvjem.html

ROLLBACK;
来源：http://hz.zhaomingkeji.xyz/gtcewjmmll.html

[Q66] 行锁查询
来源：http://hz.gogol.net.cn/gtbyfohmta.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtpcshtxpq.html

[Q67] 设置隔离级别
来源：http://hz.jinyuanbaomall.cn/gtptgvdgok.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gthjnatmnu.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtqoaevglv.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gtsuomqnak.html

ROLLBACK TO sp1;
来源：http://hz.yanxiufei.cn/gtcijjhzex.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtczgzoutb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtalvguies.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtzhttnjcx.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtuplmgsgc.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtfpffsvdf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhongyouzk.top/gtogfakedp.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtkdokhssd.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtakogztps.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtxoevsixq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenlongwang.top/gtfckhbdkz.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtkduwjkga.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtgedujogk.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtuccieovc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtuyupfsac.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtgnoalutg.html

[Q76] 按天统计
来源：http://hz.tanke756.top/gtdfykzwcv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtlummpkvl.html

[Q77] 时间加减
来源：http://hz.svipenyu.cn/gtrydfskdz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pycfn.com/gtypjtmfwo.html

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtdugulyts.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtlpjsbzie.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtuuayfotl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtaauhgfcm.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtryfkusvu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtfxrttplg.html

[Q81] 字符串替换
来源：http://hz.jinqigfzy.top/gtistusltz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtoxvwneaj.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtbkcoehpx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtmhnflair.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtwmcelymd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtdfayootw.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtvnkwxapp.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtkhzwzxpg.html

[Q85] 数值取整
来源：http://hz.dianchejie.cn/gtmrwnfvwl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtgaspiqdz.html

[Q86] 读取 JSON 字段
来源：http://hz.meibo888.top/gtntmnvqpu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtrdpupdxb.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtdrqqpqvq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fengsongda.top/gtuqdwzwth.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtrpinxkpi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cqqwz.cn/gtuowvkvvz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtxdirbjau.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtprasoaxn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtnmaphydv.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtnhteahuz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gttmaveyjc.html

================================================================================
来源：http://hz.ivvv.top/gtygpatkmt.html

R. Bash 专题
来源：http://hz.yonumen.top/gtfgfptspp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthxmodjfo.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtyykouqai.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtsfxbzpbk.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtwuvpzrol.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtwmnayknb.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtdechxhog.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gtxtefrvbl.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gttgqjsqip.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtaekuxzwf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtodrjyxkf.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtonjfpery.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtibqumplt.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gtfeoefkja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jiagoushi.top/gtbooiyafq.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtqjlwosnw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtdvwaajhr.html

[R08] 数值比较
来源：http://hz.tianlin.xyz/gtpqsdzcuv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtdiaubbsx.html

[R09] 字符串比较
来源：http://hz.aibaodan.cn/gtahcosgct.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.0kj1m.cn/gtiwsaiasg.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtcyurlbuh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.feifeiyinyue.top/gtvywvkuid.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtcjpyyqcj.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtwsttbvhj.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtmjxuhqiu.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtldcgtrle.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtwnpbiugy.html

esac
来源：http://hz.yuanzhike.top/gtbicirmpe.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gtypefylnb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtaoncjpip.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtlnfmlayh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gzhubu.top/gtuxxjpyhu.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtleuzjdsq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtjezsykdd.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtoeggbcqf.html


<!-- 参考信息 -->