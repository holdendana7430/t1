代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtqzzddjuv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtadiirjxz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtkluwblcj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gttmtncaka.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ybcxt.top/gtjnrlfxkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtsodcasns.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtfsardmcj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gtmiodfbqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gtbwozyfjt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hfpthk.cn/gtxkpxahkp.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtaofghnob.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gttgoyxrbz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtdqxbcxeo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtqjpizmvi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gthnaehvyx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtvqcszjqn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtvqdkfndq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cucudq.cn/gtywyvedql.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtigmbvemp.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtbfaxcsel.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aibaodan.cn/gtlrptflpr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtzwsilpyh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtopnrnxve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtigtcdadc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sweek.top/gthdhcgecj.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtwmveeish.html

Ruby: x.length;  x.size
来源：http://hz.chenzaomai.com/gtpwiuyaek.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.daria6918.cn/gtlbdmfvqs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtwwwdyozr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtybcnttyj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtkevvzvuq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnqzz.top/gtajeiegyd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtuqcmcuvq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtvliypzzx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yonumen.top/gtxickuzqa.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtfzwcyuev.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jlsjyb.cn/gtxwogkbpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtsdxkxksk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guannengcc.top/gtgsqyaefs.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gticnsysbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtngoehqrx.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtaqgapywy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtvksrbcfw.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtmadzysuv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sxryk.cn/gtwdptlhai.html

C#:   if (x is null) {}
来源：http://hz.9152youxi.cn/gtqaepqnsj.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtxaoqnntt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtogmofgpw.html

PHP:  // 手写时间戳比较
来源：http://hz.sweek.top/gtlhiiyvxa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtydtejnif.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gteryjabnv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtjtguscoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shuidangran.top/gtfmutjkhf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtxriqvroh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtwweukdkb.html

[P08] 处理浮点精度问题
来源：http://hz.sweek.top/gtzttoerlc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtsbbqnfne.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhijiandao.cn/gttzsxsiqi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cucudq.cn/gtktsjqyka.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtmcewwbgr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtkwvzdnvx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xziqi.cn/gtuahqjgrq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hfpthk.cn/gtcctzqokz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gthvocixlx.html

================================================================================
来源：http://hz.guowangkeji.top/gtmaiqxtpj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtqqjresru.html

================================================================================
来源：http://hz.hfpthk.cn/gtqlzroloh.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gtaenlcgwh.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtbuvmphue.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtmejsruyq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgufenzy.top/gtllfbbuif.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtonvvrlfe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtxqqxjfec.html

);
来源：http://hz.shzxlz.cn/gtrdvxauvy.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtimpgewjj.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtztqptuzv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtireagoix.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtmxkaqhiv.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtazbzdbmu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gtenxnmvdz.html

);
来源：http://hz.shanyushiyangtech.top/gtwfkxrntl.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtihdqougm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gttgrakzht.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtckthrepi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtuezbeimw.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtbzvyczez.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtqobpzlux.html

[Q06] 删除列
来源：http://hz.quarkkingdee.top/gtknnuecbd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtgweldhjd.html

[Q07] 删除表
来源：http://hz.jyoumei.cn/gtltxqeoqz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtpuqivlue.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtnucnsitb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gteqystabt.html

[Q09] 创建唯一索引
来源：http://hz.c1oappe.top/gtdffytsjg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtpptqpooi.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtiyyfdcou.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtowgyffdo.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gthnfabukw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.snrcjt.cn/gtdzrhkjxb.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtbmsgyoow.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ppjwa.cn/gtybovauve.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtwnjfjent.html

[Q13] 忽略重复插入
来源：http://hz.hongshengwenyu.top/gttjajrcof.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.mhx1999.top/gtblhkydaw.html

[Q14] 存在则更新（upsert）
来源：http://hz.pengpengdd.cyou/gtiskjvjfu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenlongwang.top/gtuenytkcm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jianghu66.top/gtamkqbowq.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtolzszzty.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtwrmyfgjj.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gtadvobkdb.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtjpinggau.html

[Q17] 条件查询
来源：http://hz.gotoacloud.top/gturgjzqgl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangtech.top/gttvebymgt.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gtwbwqcnop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangshuangyany.cn/gtcgdhwytc.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gteeesqjcg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtndrvzobp.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gtgblkgnft.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ppjwa.cn/gtkjugealm.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtahxqciws.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj202588.top/gtaejmlhmi.html

[Q22] 排序
来源：http://hz.meibo888.top/gtsrbvmqqk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gteimehrhk.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gthwtrqyku.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtqrykhrqn.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtbprwtqga.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtoxglpqip.html

[Q25] 只取前 N 条
来源：http://hz.xingfuxueyuan.xyz/gtzayuytst.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sufxvd.cn/gtbbsspsca.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtaucqmsha.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtjoxltjyu.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtfyemtvyl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtiwamwyro.html

[Q28] 求和与平均
来源：http://hz.wangshuangyany.cn/gtaqgkddsa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtawbpegel.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtrlxykttu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtturvwkaj.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gthsjndzfe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtgnpruwdq.html

[Q31] 分组后过滤
来源：http://hz.zhaomingkeji.xyz/gtppcqqknf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtzwsffosv.html

[Q32] 分组拼接字符串
来源：http://hz.andypj.xyz/gtznlsdpue.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtlgrdyddg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.andypj.xyz/gthzmcnggf.html

[Q33] 多列分组
来源：http://hz.hysaishi.cn/gtsuynnkqa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtojpdmnib.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gtryrbgadj.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtspmyxcjh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtrhyshznw.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtaxnedmbl.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtnpjajxkh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtwrcfvukl.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gthlitnmdc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gthwxyddyr.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gteqnzjjtg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.redwolf501.top/gtbgkwxntz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtsdyyeegv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hammf.cn/gttvfqzkhr.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtsahixhhb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aizwys.cn/gtgtvruwmo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.redwolf501.top/gtaecqaqjk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtqdqigqix.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nwbrower.top/gtmhmblpjt.html

[Q41] 多表连接
来源：http://hz.nwbrower.top/gtjbmkshdr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtlndemvwa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtdvvfwhyk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydzc1.top/gtbdckzgfn.html

[Q42] 连接条件附加过滤
来源：http://hz.yuanzhike.top/gtmcqubbuj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtcwhwdezt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtcrpdexzg.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtltsyfgfa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtbhfeunnf.html

[Q44] IN 子查询
来源：http://hz.haohaochexian.top/gtvjjkxapg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtulfndgax.html

[Q45] EXISTS 判断存在
来源：http://hz.feifeiyinyue.top/gtsrryocxt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtsgjykxwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.0kj1m.cn/gtdskfmlhj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtqdlfvoaz.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtxqaroqmy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shuidangran.top/gtmkhunbpc.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigfzy.top/gtyepyognk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtesqexpym.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtqzhuvjlb.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtskhvkysw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtydgvktui.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gthwwammks.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtffnlnirs.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtgyocvsfo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daxiang520.top/gtiuxgmgzs.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gtgapeetrr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.smart0.xyz/gtcodziyuk.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtgwlqwepi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yvedp.cn/gtqkcgxiti.html

[Q54] 清空表
来源：http://hz.jlsjyb.cn/gtxvuckfoc.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gtgqekygqa.html

[Q55] 排名（并列占位）
来源：http://hz.vqdsnc.cn/gtipidcdgw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtulrtovcm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtzrdkgzrb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtirzpxhnt.html

[Q57] 行号
来源：http://hz.yj202588.top/gtiuywputm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtxgcucsfb.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtggppmwei.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtloxozpml.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtodvcjctl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtdvlyeznt.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtiasfvsnr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtmeprrref.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtorptmhnp.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtnhpjbiat.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtxttfpydq.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtwjcrizcc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtpdaugegs.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtwfqpxpmw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtjdqpjlic.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtxwsgbyhv.html

COMMIT;
来源：http://hz.chenzaomai.com/gtmvcfjajs.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtosjixpfu.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gturbmegll.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtkcxhffri.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtywqlegri.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtbtjxjpen.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtixtwvzwq.html

[Q68] 保存点
来源：http://hz.ybcxt.top/gtkedshjjo.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtezcuisqn.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtptpdcmek.html

[Q69] 查看执行计划
来源：http://hz.tianlin.xyz/gtafcrkgga.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gtyhiyzknq.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtnwkmkpuy.html

ANALYZE TABLE users;
来源：http://hz.xziqi.cn/gtkvjoptsb.html

[Q71] 查看建表语句
来源：http://hz.chenzaomai.com/gtshbxgczk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtsqfbqxzo.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gturpdvorw.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtftkdxvkh.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtaraxnnmo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gteuzgsede.html

[Q74] 强制使用索引
来源：http://hz.guowangkeji.top/gtlehbudbc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yanxiufei.cn/gtufroyhpc.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtsbubssdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtelkfmjpw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtspvqrgci.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtanjontls.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtiiawttqh.html

[Q77] 时间加减
来源：http://hz.shuidangran.top/gtrjbnbjlv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cdnleiting.top/gtxvotuodc.html

[Q78] 当前时间
来源：http://hz.shzxlz.cn/gtqvtmaeja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gtjuwvbecd.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtagopryqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtmyyedgmq.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtqfflvpcp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtwexwkgyq.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtrzvferul.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtzbhswtzk.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtpquddpka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gthjbvtflf.html

[Q83] 大小写转换
来源：http://hz.xuanzx.com/gtlnycrodl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtroosjbij.html

[Q84] 去除首尾空格
来源：http://hz.ydjk.org.cn/gtriyqebzk.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtavsyhmtn.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gttjuqcvtn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhengqikj.top/gtpcgdyadd.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtvujwmxkk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtewznoqfw.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtgwqgmerf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhiwuduotai.top/gturkelwyg.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtdnwgemnh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gtabyfrvpx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtqzntkizz.html

[Q89] 判断表是否存在
来源：http://hz.andypj.xyz/gtaxtkkvuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtpmiqrutm.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtohfbtzwm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtbhlpjgnq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtakbhmvjo.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtmphtkwht.html

================================================================================
来源：http://hz.tanke756.top/gtbnfkywyl.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtzycjmzqc.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtisdscjhc.html

set -euo pipefail
来源：http://hz.yonumen.top/gteuljtuzb.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtkiwqudsi.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtcuvwvzut.html

[R03] 只读变量
来源：http://hz.chenzaomai.com/gtcrcqouwj.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtwusjgdcl.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtqbzfvjdz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtsywepchb.html

[R05] 参数默认值
来源：http://hz.nwbrower.top/gthtroauaq.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gthenecpwf.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtstgwzcav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtowawiapf.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtfekfisjj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yonumen.top/gttliluber.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtotzaolvs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sysykeji.top/gtdtfnayic.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtznwdxpyy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtgnzedmbd.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gtuzfvoigf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtntrelvhl.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtudyemysj.html

case "$1" in
来源：http://hz.ydzc1.top/gtmnjcvqin.html

start) echo "启动" ;;
来源：http://hz.xingfuxueyuan.xyz/gtjnufbgsq.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtcjivofmw.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtykzmkuxf.html


<!-- 参考信息 -->