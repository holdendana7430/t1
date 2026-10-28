代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtsidnrdim.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtcfqbgtmm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtbkugzbwh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gthygmbkbd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.vqdsnc.cn/gtczcrzhrv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.kuanghao11.cn/gtxgmfqgib.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gtluaoztfu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtkjbvpsxl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.iojbl.cn/gtyonhvaef.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gthhocojib.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtbanjzhya.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gtnleoobxv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenzaomai.com/gtlnuhqchc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtzuiiuqza.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtykahmvvo.html

[P04] 求长度
来源：http://hz.52xcode.cn/gtcgmaxtzz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtcsjznolt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtljnxgqww.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtcifulwlu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtqrtupvzj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtfwuouhxb.html

Go:   len(arr);  len(m)
来源：http://hz.yj202588.top/gtueukpesk.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtsxcgvezb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtauoejdyr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtmgfgnjaq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtclprlmqo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gttlfvmlyo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtawouekvw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtxkxsxhsa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gtyvblkyns.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.svipenyu.cn/gtlqdaawxd.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtklhjzkgr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtaqgvjpuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gthnmdihxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtxdtssxxt.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtfjblsmwq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hongshengwenyu.top/gtplilaymo.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gtggfxpxcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtozkfmjjp.html

Go:   if x == nil {}
来源：http://hz.cashguo.top/gtwykrldqq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guowangkeji.top/gtplshfjvc.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gthogbmvtn.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtuwvblzrc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtsaeqhfbe.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtxfcpjxhc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtppadkpvt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtlexmeauh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtlshukctl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhoulong.xyz/gtlkebsnis.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtgvoxpxvb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxuanxn.top/gtcqqikjjm.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtamauzpjn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnqzz.top/gtyszothyq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jlsjyb.cn/gtjuwbwhgs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gttvdaegcu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtglpnynpm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtloqjslhm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jyoumei.cn/gtunsiezrk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtbuxkwren.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shuidangran.top/gtojlounxr.html

================================================================================
来源：http://hz.cheryme.top/gtgsctiwjj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtqyssfnwk.html

================================================================================
来源：http://hz.yangfankeji.com/gtbljcnwnl.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtfdexeffa.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gtemvbshss.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gttpuqfwxl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtreuybtwm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtzemorxqq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gtkkfgdnjt.html

);
来源：http://hz.jiagoushi.top/gtpgbbpzjf.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtscxppymi.html

CREATE TABLE orders (
来源：http://hz.yangfankeji.com/gtphwkevbq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtommqpemt.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtrgtdljpo.html

amount DECIMAL(10, 2),
来源：http://hz.yuxming.cn/gtluujbvnt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gttpzgymnb.html

);
来源：http://hz.fzhhl.top/gtuwtqdile.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gtqpzvnhnm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuanzx.com/gthnhdxzqd.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtmhgmdgxx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gtmvbokjeh.html

[Q05] 重命名列
来源：http://hz.zhongyouzk.top/gtswhpqycc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtqswvcgxz.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gtukvvsytb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtvswxyhnc.html

[Q07] 删除表
来源：http://hz.sweek.top/gtwknsnmge.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtlgjcvcdr.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtzauumcka.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtyvhvmvjq.html

[Q09] 创建唯一索引
来源：http://hz.yuxming.cn/gtnqoxefve.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtxqrjhcho.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtxjzhrthl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtvvrgubbt.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtinllzabz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnqzz.top/gtbbsjxupk.html

[Q12] 插入后取自增 ID
来源：http://hz.jinyuanbaomall.cn/gtrjmhhbxd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtlcnrchgm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtylhtjgmr.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtcjctldsq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuanzx.com/gttvvrikvl.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtjwdgtwgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zdqjudy.top/gtbvqmqjic.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtdsbiehpt.html

[Q15] 查询全部
来源：http://hz.birdmap.top/gtvejzdujo.html

SELECT * FROM users;
来源：http://hz.ydzc1.top/gtwwzpdiwc.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtxvkozwqg.html

SELECT id, name FROM users;
来源：http://hz.ywan-chungtsiang.top/gtsczgrezu.html

[Q17] 条件查询
来源：http://hz.nanxuanxn.top/gteelpplvj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pengpengdd.cyou/gtsfyulgyj.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtmttruhpg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtxkyvydbj.html

[Q19] 范围查询
来源：http://hz.shuidangran.top/gtgmxtehtb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtxgyabjaa.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtvtvftijc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuanzx.com/gtbkegfmhu.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtquoznazu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtjwejbqtt.html

[Q22] 排序
来源：http://hz.9152youxi.cn/gthzbfflxa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtbgqskhbf.html

[Q23] 分页
来源：http://hz.ydzc1.top/gtvgstlzah.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtbgnppnku.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gtefxiroic.html

SELECT DISTINCT city FROM users;
来源：http://hz.ivvv.top/gtfqblzuig.html

[Q25] 只取前 N 条
来源：http://hz.jinqigfzy.top/gtproqysnz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtnjpwwnjl.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gtkewqdepu.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gteoqxzjbu.html

[Q27] 条件计数
来源：http://hz.yangfankeji.com/gthwnxklud.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ybcxt.top/gtmzyokcnn.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtzydqyzpb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangshuangyany.cn/gtnfotukca.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtwxipsvdi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daria6918.cn/gtpdixltsm.html

[Q30] 分组统计
来源：http://hz.shangyingyoupin.top/gtdwhhqvdt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtttfgwxct.html

[Q31] 分组后过滤
来源：http://hz.bjfxy.top/gtomxiaoen.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtydmunyik.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtaqdbpsjy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtpioqqxxe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gtquxwwkfg.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtbvfrwqno.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.mhx1999.top/gtanyicdop.html

[Q34] 每组取第一条
来源：http://hz.ywan-chungtsiang.top/gtwsonbkhb.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtygqzpaia.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtkljyixjz.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtsebyugew.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtevvwnqto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtgtfvgbmf.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtgejtoclr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtbzxarqak.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtbwghsixg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zdqjudy.top/gthllagxsy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtfescsidt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtcuyyptzx.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtdrfelyoy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gthimbkkbi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gotoacloud.top/gtmwwipgzp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnxiangtu.top/gtiwpwkkvh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtuuakstim.html

[Q41] 多表连接
来源：http://hz.zhoulong.xyz/gtafwwmcbf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yueranfly.top/gtouaiawsy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxinkj.top/gttttfemxp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtjelduonn.html

[Q42] 连接条件附加过滤
来源：http://hz.yongpay.top/gtqdfeivnt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtomtebour.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtihqtirxl.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtaawvmskw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtcbcdhnca.html

[Q44] IN 子查询
来源：http://hz.fzhhl.top/gtlmhgpayw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtannkcjwl.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtwumcdbla.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtxlfhefxy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhijiandao.cn/gtqgjimzec.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtzbqztbyk.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtkgijtxkb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.9152youxi.cn/gtkmadzxny.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtecqjtdmr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dianchejie.cn/gteyhrnabh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtdiaosfix.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtdtguphlf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gttdvnnuhv.html

[Q50] 批量更新
来源：http://hz.tian-w.cn/gtdfuxamyb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gthdjoywcx.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gthosivxhj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtjlcsioba.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtzljgdghz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gtglrvdxil.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtpchfnojs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtrtpdnbpk.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtcnzxfcst.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangtech.top/gtrmfumemd.html

[Q55] 排名（并列占位）
来源：http://hz.ydzc1.top/gthbtpsixa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtywyysmdh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtwlvzxssk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gtuhrdvaro.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtpbuscdcz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fengsongda.top/gtqdnjambg.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtbkprnstu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtaymxqlch.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gthytfpajd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cdnleiting.top/gtrdqysodv.html

[Q60] 取上一行 / 下一行
来源：http://hz.tian-w.cn/gtkntaunwb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhengqikj.top/gtbajxxsiq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtiyycownf.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtavaekjsq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtwrvbcxzk.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtuaxiyqhr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtgbrldtzf.html

[Q63] 开启事务
来源：http://hz.kuanghao11.cn/gtgvuazkgd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guannengcc.top/gtaiodzesk.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtmiukjjzl.html

COMMIT;
来源：http://hz.gogol.net.cn/gtndmkrekr.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtdkguufer.html

ROLLBACK;
来源：http://hz.hywenlv.cn/gtchxlalqo.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtwovpejut.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtbgiinxkf.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtsshwxthg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtwzyjjism.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtwnubmbgh.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gtwxigckwq.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gttgappskt.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtwoevqfwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtpuxlqili.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gtfbmyqafv.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtasjvrtmg.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gthgdknbri.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cashguo.top/gtmvbpanxe.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtomkwezfa.html

SHOW INDEX FROM users;
来源：http://hz.shangyingyoupin.top/gtqsxksjgs.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gtrtsjplcj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yueranfly.top/gtfyhbnvqi.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gttxvdyliu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtdhubfeda.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtakgckpqr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gthnljlzwg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtqgsfgaqs.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtijcbedtr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daxiang520.top/gtosqmpgfx.html

[Q77] 时间加减
来源：http://hz.dashuyun.cn/gtgygbzdlj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cucudq.cn/gtwfzgwfsn.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtultmqewp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtdrlemzmg.html

[Q79] 字符串拼接
来源：http://hz.haohaochexian.top/gtrlzwkzpe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtycubbcam.html

[Q80] 字符串截取
来源：http://hz.ydzc1.top/gtxothlhci.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtdmlbpzru.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gttveclhtx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtahnygryw.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtlsbwskhb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jyoumei.cn/gtnldwyqmk.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtnqggomqd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ppjwa.cn/gtzvchcxbz.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtogwoqsft.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gtpppfuswb.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtkynzpolz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtixqoqtxp.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtmzfrjsbh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtkkfxngyj.html

[Q87] JSON 字段做条件
来源：http://hz.gzhubu.top/gtwddvmoxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtuzmasmhz.html

[Q88] 行转列（条件聚合）
来源：http://hz.yongpay.top/gtrtfbuoft.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtzkpsloxe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shuidangran.top/gtzruvgpxf.html

[Q89] 判断表是否存在
来源：http://hz.zhongyouzk.top/gtezejchoe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gtheddxhqm.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gthscaynas.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.smart0.xyz/gtsxbtsncb.html

================================================================================
来源：http://hz.hammf.cn/gtcttrxmyh.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtyppnhfrj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtpihpzlmv.html

[R01] shebang 与严格模式
来源：http://hz.hammf.cn/gtcocrrmcu.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtiggmljor.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtthzecxjo.html

[R02] 变量赋值与使用
来源：http://hz.dashuyun.cn/gtaatvacyt.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtqdnuwrmw.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtgedkispe.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtjsjxkvov.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtxiliqgmo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtxkkuwsjv.html

[R05] 参数默认值
来源：http://hz.jlsjyb.cn/gtakagfdfy.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gteruuywcw.html

[R06] 判断命令是否存在
来源：http://hz.ivvv.top/gtqmcwzbao.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtbwdxwpri.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtybjvqwvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtbsslbkqm.html

[R08] 数值比较
来源：http://hz.yvedp.cn/gtfsnxugzc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtfjmdxdtb.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtvckxhfpj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtfijbpoug.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtgnjnjknm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtksuyiqxm.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtpapxtndx.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtrnyihxfx.html

start) echo "启动" ;;
来源：http://hz.gogol.net.cn/gtdcknuthw.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtpbgfacxk.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtqslrrqvv.html

esac
来源：http://hz.chenzaomai.com/gtjmliuxvs.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtsshbrmoz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtygqcwowu.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtsxpghlar.html


<!-- 参考信息 -->