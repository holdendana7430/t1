代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtufsxqdtj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtvklqbmtc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtsjhpdpid.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtysanhkon.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtskptypnk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yanxiufei.cn/gtjpnrdbsd.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtzcacbwgd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhixingplan.top/gtfhacgyxh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cucudq.cn/gtmcotwdme.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtclsatqop.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtdwaoiawu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtgoyzyoww.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenlongwang.top/gtdaqfsinj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gtqixuhlpu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtzdmeolqr.html

[P04] 求长度
来源：http://hz.andypj.xyz/gtiklmling.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtopwobocr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtynmrtwgd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtejqkfbsx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtjmvbnvsf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gthkyhgtfx.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtcgzngwil.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gtqihbkgoq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gtckbsfrsc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtwxpdagsz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtaovdmhmq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtiawbwxlw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtubbrhqlf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtpyyymszk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtrlgfexxa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtibmnsoos.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtbwwrbscl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zycfv.cn/gtnunlnjnf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtsxeehojj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ywan-chungtsiang.top/gteghpvmyk.html

PHP:  if (empty($x)) {}
来源：http://hz.yuanzhike.top/gtdnfgbsvz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tanke756.top/gtgpdybvou.html

TS:   if (x == null) {}
来源：http://hz.xuetiantiany.cn/gtelquvnkx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gteabsqvou.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtsvbqyykl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhixingplan.top/gtwkiqkaxw.html

C#:   if (x is null) {}
来源：http://hz.zdqjudy.top/gttlfrtmoz.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtaxhwrouv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtarbmjiyj.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtrmbnksxk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtcdrcsabi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtrfxbrzug.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtpamzgesl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtablyobgz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xylfe.cn/gtwkycxubs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guannengcc.top/gtiwcqqzrn.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gthhalfcvl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtnhakhnaw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtmkgtnqal.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtstgceadg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.c1oappe.top/gtbzbegivz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtnwfoiqzr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtobrfckrt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtsoouqdjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gttjgcwgyz.html

================================================================================
来源：http://hz.hnxiangtu.top/gttiuctnsv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtexkjdjko.html

================================================================================
来源：http://hz.daxiang520.top/gtlfgdpfdr.html

[Q01] 创建表
来源：http://hz.yonumen.top/gtigtmolfb.html

CREATE TABLE users (
来源：http://hz.tanke756.top/gtfbpsopfz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtapcdvwoi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj202588.top/gtfhxasrsa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhixingplan.top/gtmnnydiof.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cucudq.cn/gtakwflzsm.html

);
来源：http://hz.smart0.xyz/gtdrhfgbwt.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtpqrmuvvh.html

CREATE TABLE orders (
来源：http://hz.jqgufenzy.top/gtmoyvvwlg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtzmzozfuo.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtsugnymff.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtfdvwawkj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtsciagvmr.html

);
来源：http://hz.tian-w.cn/gtihdmnigw.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gtbxgcquwn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtukizcpkj.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtpiointhb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangshuangyany.cn/gtwuqneylk.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtnoofzbuc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtfitrqvyo.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtoqwdkyny.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nwbrower.top/gtokwpbbay.html

[Q07] 删除表
来源：http://hz.pengpengdd.cyou/gtfquiyanx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ybcxt.top/gtokvoibgb.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtrcnjypod.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtvplhbhmc.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtcqnwaosj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gttkxyuuqh.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtdcekhssj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.52xcode.cn/gtuwyyknep.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtkaxbacar.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtojqijrxd.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtctmjvtzt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gttmhlbgxt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.snrcjt.cn/gtmmzuypyj.html

[Q13] 忽略重复插入
来源：http://hz.cashguo.top/gtltdupiah.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guannengcc.top/gtbxfwpipg.html

[Q14] 存在则更新（upsert）
来源：http://hz.pengpengdd.cyou/gtdehwxtyw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hywenlv.cn/gturjxueac.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenlongwang.top/gtbdcsnaga.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtvylcvfpk.html

SELECT * FROM users;
来源：http://hz.shzxlz.cn/gtxypvzsrx.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtagpzkljz.html

SELECT id, name FROM users;
来源：http://hz.yj20258888.top/gteglmozqa.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gtkiiuskwb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtcfgxdovh.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtonyburus.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gtugmphtom.html

[Q19] 范围查询
来源：http://hz.hysaishi.cn/gtodxbyhkv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtkqykndhd.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtzergpyzx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gthlumcybh.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtctauvgxn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtbxczkapn.html

[Q22] 排序
来源：http://hz.ydjk.org.cn/gtqyhfdrhs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtolrhxfws.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtixhvwvzk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gtoqzhwmyv.html

[Q24] 去重
来源：http://hz.meibo888.top/gtpwesthmo.html

SELECT DISTINCT city FROM users;
来源：http://hz.tianlin.xyz/gtfpzetswj.html

[Q25] 只取前 N 条
来源：http://hz.yj20258888.top/gtauqttjrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtmptgecyz.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtspsocdox.html

SELECT COUNT(*) FROM users;
来源：http://hz.jyoumei.cn/gthzrkctpx.html

[Q27] 条件计数
来源：http://hz.aizwys.cn/gtxtruoluz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtxnnfcdyn.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtztrpruoq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtigjskmpj.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gtvmsnsaxg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtoltfrcmj.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtmoisvhuy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtumbldpjx.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtpvuysrjo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gotoacloud.top/gtjozhjbkv.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtmflfxmla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtfmurippm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ehwqpu.com/gtbazmihrb.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtswpbunkf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtcrajlihx.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtxiawlprs.html

SELECT * FROM (
来源：http://hz.meibo888.top/gtagvpptmv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtwwrqgadn.html

) t WHERE rn = 1;
来源：http://hz.hysaishi.cn/gtmkcpavnr.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtxwhmancx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtzcadubxn.html

[Q36] 左连接
来源：http://hz.iojbl.cn/gtbmyibyke.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtvsvnveyz.html

[Q37] 右连接
来源：http://hz.hywenlv.cn/gtlhkezlpt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtxrqyzmwm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gthzjsgeyc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtiuudhojx.html

[Q39] 自连接（查上下级）
来源：http://hz.tianlin.xyz/gtnnzzofml.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtyxdcvnjp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtamquhmdb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnxiangtu.top/gtgvzwjzdp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gtlxziyjvc.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtpyldjlgz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtwreglden.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtmdhduwpb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtgjgajrdr.html

[Q42] 连接条件附加过滤
来源：http://hz.jyoumei.cn/gtnsuwzowz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtuqiojgjt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtulxpbtvf.html

[Q43] 标量子查询
来源：http://hz.daxiang520.top/gtiutmlxgb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtjajehhxy.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtponjpeof.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.bjfxy.top/gtozdhcsbl.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtprtutacx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtydhfamsg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.svipenyu.cn/gtpxxzqiek.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtwuokdxwi.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtouzkmyrp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangtech.top/gtpldbtggb.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gtlvcufshh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnqzz.top/gtuhkodgmg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtcsxtxxsq.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtztxarnju.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtbpzqvcgf.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gthlttkgui.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtuotxyduo.html

[Q51] 用子查询更新
来源：http://hz.quarkkingdee.top/gtxqrnmerw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtifseohdb.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtzmagxsgr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtpmdfkxbs.html

[Q53] 按条件删除
来源：http://hz.yuanzhike.top/gtajmpbfxh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtkgwgtzkn.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtxpmnylpk.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gtjqaiatpz.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtpisahbem.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtbgefoalz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sufxvd.cn/gtosjjjdpz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtpjighvex.html

[Q57] 行号
来源：http://hz.xuanzx.com/gtbojdxrua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.redwolf501.top/gtjbeolujm.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtqjecuixv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtvgmhglkt.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtfzanwguw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtjzgdszhw.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtarpridxi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtankyrkfu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhongyouzk.top/gtnkcuwtxq.html

[Q61] 移动平均
来源：http://hz.redwolf501.top/gtrskpygur.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtqbpaedan.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gttakwgxmf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtdxeywrvi.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtqmwdpkgh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtvaqkoftg.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gttqhbgoqq.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtffglixnp.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtmkilakue.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtpunyejni.html

[Q66] 行锁查询
来源：http://hz.jiagoushi.top/gtrvzrwbsq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtrebjbugp.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtvsghztzr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtddwhazic.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtgtwsivpg.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gthlfelcjm.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtfcjopkdq.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtcnftuwtr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gthycpeshg.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtqqkunelr.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtdmywdllx.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtjltzwprv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gtqdoxsjsa.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtnvapbriy.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gthyhxfjme.html

[Q73] 查看表状态
来源：http://hz.jianghu66.top/gtljyhauug.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtzuaqjkkc.html

[Q74] 强制使用索引
来源：http://hz.kuanghao11.cn/gtopcyjauk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtlhpoqdcw.html

[Q75] 日期格式化
来源：http://hz.fengsongda.top/gtegilmkey.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gtejipeycp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigufen.top/gtysslszdm.html

[Q76] 按天统计
来源：http://hz.birdmap.top/gtjhddpuwe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtssniwvcr.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtovoaztsc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtmqegiinz.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtzxjvfcvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtszjyqwac.html

[Q79] 字符串拼接
来源：http://hz.shzxlz.cn/gtnimgrsru.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtlogcrbzy.html

[Q80] 字符串截取
来源：http://hz.svipenyu.cn/gtulrcacvn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtyltinlga.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gteqnvreed.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtslyvfcxc.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtdbmatzfn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gaohongyu789.top/gtcxacdaxx.html

[Q83] 大小写转换
来源：http://hz.gogol.net.cn/gtdkbqrsis.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtrmchswxa.html

[Q84] 去除首尾空格
来源：http://hz.tian-w.cn/gtornmhyrj.html

SELECT TRIM(name) FROM users;
来源：http://hz.jianghu66.top/gtjspmdcac.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtlzylcjbh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtaptlbdvy.html

[Q86] 读取 JSON 字段
来源：http://hz.daria6918.cn/gttemoekjp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtpdimqkqz.html

[Q87] JSON 字段做条件
来源：http://hz.xuetiantiany.cn/gtjpxgsesy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtcmywnuhe.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtztvoaiyq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtzdjygwzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtsxvgqlda.html

[Q89] 判断表是否存在
来源：http://hz.yangfankeji.com/gtmgealhvs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtzduaicrb.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtcwrezeij.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sysykeji.top/gtbdqlidlv.html

================================================================================
来源：http://hz.316326.xyz/gtsjefggcp.html

R. Bash 专题
来源：http://hz.ivvv.top/gtjmrfouwq.html

================================================================================
来源：http://hz.wangdashe.top/gtcdxahwqv.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gteglnokys.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtomctweyu.html

set -euo pipefail
来源：http://hz.fengsongda.top/gthshxuxps.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gttmopjhwr.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtdgogxvvp.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gthacdugwu.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtlaevgtzw.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtyhqgkmau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtegbbtnyx.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gtzzhqvmlk.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtxrjguhmc.html

[R06] 判断命令是否存在
来源：http://hz.xingfuxueyuan.xyz/gtcgygpfoo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtualimoeh.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtknxxfksi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtphnavxif.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtuovbsxsq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtplwbtaxk.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtfwhgkkgp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtryhzqkin.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtgcjarjbq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gtdgkyhkhg.html

[R11] case 多分支
来源：http://hz.jqgufenzy.top/gthizjcsxg.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtuhzdjhcf.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtetcmpvew.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtkpgwmync.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtoasxnoef.html

esac
来源：http://hz.yanxiufei.cn/gtnmytddrx.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtabrwpefc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtbwtdcrqy.html

[R13] for 计数循环
来源：http://hz.mhx1999.top/gtcuteblok.html


<!-- 参考信息 -->