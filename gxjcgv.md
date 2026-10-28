代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtqdjiuskt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtrptlffnd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtcfcevhsd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtygimleik.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jianghu66.top/gtdvekzhph.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhiwuduotai.top/gtyssxvmmq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtdjybqzlj.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gttplcamxd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gtqeyaozzc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtvpohwsio.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtsuzuuvwf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtdvrxjdje.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gtdfnnsqtw.html

Go:   len(arr);  len(m)
来源：http://hz.daxiang520.top/gtjkspujxc.html

Ruby: x.length;  x.size
来源：http://hz.zhixingplan.top/gtzbrjlyuj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtjmmezctu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtcjqscrta.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtkocxgmix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtdwjoufku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtsoguustc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtvwtyabtz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuetiantiany.cn/gtehichvor.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtcukguksf.html

Ruby: a == b
来源：http://hz.ybcxt.top/gtkfvcjpqj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtzfmdvogq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtirmlhmoz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtxqwcojqn.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtnxewlnlk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtuumplfgk.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtghhhxzqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtqmefsxte.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtxdwlkezm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gthgfwknmb.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtyinbpwpn.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtxoxvjyen.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtcaclqwpf.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gttmexivuc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtigbkcnxr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtmkmzoczb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtannzahss.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydjk.org.cn/gtyozoulrq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtbajjeqdk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtbqabvlnv.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtszsllxkt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sufxvd.cn/gtewwbjjid.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gtiwamefxr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtottntcrt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtioecrudv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtqhzigknu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ivvv.top/gthvskjnoo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtfhnhwmpo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xingfuxueyuan.xyz/gthgmnqlwg.html

================================================================================
来源：http://hz.sufxvd.cn/gtilzzwgro.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtbxflkzfm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtejelssqx.html

[Q01] 创建表
来源：http://hz.hfpthk.cn/gtesmagntt.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtviawsyco.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtigbnibcc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtglqknpgf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yvedp.cn/gtnskvpmua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cdnleiting.top/gtolchnkrq.html

);
来源：http://hz.wangdashe.top/gteuswehld.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gtmgpowokf.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gtbxyzcuiv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtspuklfws.html

user_id INT NOT NULL,
来源：http://hz.meibo888.top/gtocbpdrge.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtirwaexrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.iojbl.cn/gtyclwjpkr.html

);
来源：http://hz.cashguo.top/gtdjwlidnz.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtdzxmwwwj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtkcionkqb.html

[Q04] 修改列类型
来源：http://hz.shzxlz.cn/gtjykwjilb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhongyouzk.top/gtfmrfbxsb.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtlimslwae.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtnnweizkg.html

[Q06] 删除列
来源：http://hz.xuetiantiany.cn/gtikeucxnn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.haohaochexian.top/gtoenyyfyq.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtwkormzas.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtimrbtacv.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtgnflqoju.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtnlhnxgfn.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtocbzvuem.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtpkqqxyyd.html

[Q10] 插入单行
来源：http://hz.dashuyun.cn/gtedhqaxar.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gzhubu.top/gtatsmfidv.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtqbejslgq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jianghu66.top/gtdppjuikq.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtuukudmon.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jianghu66.top/gtomsnymtw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pengpengdd.cyou/gtgroexkmv.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtqyiwitdj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtslejgwta.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtzdmkpwtt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tian-w.cn/gtbcuxrvll.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hysaishi.cn/gtdpqxhckb.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtbhhmfqpr.html

SELECT * FROM users;
来源：http://hz.redwolf501.top/gtbpmfqtlm.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtzjhycekp.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gtoxymwsjp.html

[Q17] 条件查询
来源：http://hz.zhongyouzk.top/gtfkcuxtxd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinghuilouyu.cn/gtorfevycm.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtghalzjxt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sweek.top/gteklfzkfk.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtuayytwqd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258888.top/gtcgtfnmdk.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtbosfwlpw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtumugymet.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtqdemdzgf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gtzrtxokcj.html

[Q22] 排序
来源：http://hz.chenjidiqi.icu/gtqmroskcj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gotoacloud.top/gtzoqscmgc.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtxnwseiev.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinghuilouyu.cn/gtsfqkxkfo.html

[Q24] 去重
来源：http://hz.yongpay.top/gtgxengolr.html

SELECT DISTINCT city FROM users;
来源：http://hz.smart0.xyz/gtlovysaht.html

[Q25] 只取前 N 条
来源：http://hz.aibaodan.cn/gtbuytpqvr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gtkbfmtubt.html

[Q26] 计数
来源：http://hz.sxryk.cn/gtrakhrlld.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtsdttoavt.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gttvntwpaa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtecnotjra.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtsjnccyqc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtkvfeptzt.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtbbdonnfx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtntamwjdc.html

[Q30] 分组统计
来源：http://hz.yj20258888.top/gtmoidypho.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtazptvpbu.html

[Q31] 分组后过滤
来源：http://hz.yj202588.top/gtxevyattf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtcfnhdnsb.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtzcbjsogd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gteilzpqoh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtfhnbkjbb.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtdytbulas.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtnzicewde.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtjtiptpmu.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtwtwombin.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtilzviylo.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtuxymnycj.html

[Q35] 内连接
来源：http://hz.andypj.xyz/gtbajulcpv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtccvdklxa.html

[Q36] 左连接
来源：http://hz.shanyushiyangtech.top/gtghigomrh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gtqcdrtnls.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtydcjhivr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtwlaojyyi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhaomingkeji.xyz/gtoqhymmqk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gthznmjdvn.html

[Q39] 自连接（查上下级）
来源：http://hz.sysykeji.top/gtlkhwukxm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtwkfpwewh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gtdiepllrd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.quarkkingdee.top/gtbuihhncy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtrctjavam.html

[Q41] 多表连接
来源：http://hz.gzhubu.top/gtvujtxfzx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinghuilouyu.cn/gtiksdlhhb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtvkbxjqru.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtriknxfhn.html

[Q42] 连接条件附加过滤
来源：http://hz.tanke756.top/gtryhvdybk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pycfn.com/gtldlbzskk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtamlyxtki.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtltjvshzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtlpknvmnt.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtrxvockqp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sxryk.cn/gtgbwqmrgr.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtswepjbtn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gthskzwxmc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtwapjfvxy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtfdcpgoqs.html

[Q47] 与平均值比较
来源：http://hz.zhengqikj.top/gtcbdfuexb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtvgkrnvpk.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gtigrnxsri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sysykeji.top/gtxhevirmx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtpiyznjdd.html

[Q49] 更新单行
来源：http://hz.aizwys.cn/gtmvgdrgca.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtwvmdcscc.html

[Q50] 批量更新
来源：http://hz.hfpthk.cn/gtgyvticbr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.redwolf501.top/gtajyvamdw.html

[Q51] 用子查询更新
来源：http://hz.yuxming.cn/gthhkadlng.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangshuangyany.cn/gtflbnvizt.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtlpgcopun.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtrkzdtuoc.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gthdaoncru.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtbgsxtuxo.html

[Q54] 清空表
来源：http://hz.ywan-chungtsiang.top/gtcfhnukeo.html

TRUNCATE TABLE logs;
来源：http://hz.daria6918.cn/gtpgiypapg.html

[Q55] 排名（并列占位）
来源：http://hz.zhoulong.xyz/gtitccqigy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gttvmrzcvc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtbwlmrnwt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtvinpksbh.html

[Q57] 行号
来源：http://hz.bjfxy.top/gtfwfxiouo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtakgtykxf.html

[Q58] 累计求和
来源：http://hz.zdqjudy.top/gthmnkkjbs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtvwtermgy.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtlbjbxlcu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtvhifjdsj.html

[Q60] 取上一行 / 下一行
来源：http://hz.smart0.xyz/gtgblozitl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtdqdvuxuf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtogrjftli.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtawrckrml.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.quarkkingdee.top/gttkwtshwc.html

[Q62] 分组占比
来源：http://hz.sufxvd.cn/gtpnxsrgzy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtckzbmrwh.html

[Q63] 开启事务
来源：http://hz.daxiang520.top/gtblwosdow.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gtzukypjpr.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gtsgvtfial.html

COMMIT;
来源：http://hz.cucudq.cn/gtbixlfbpb.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtlwnmjwpi.html

ROLLBACK;
来源：http://hz.cdnleiting.top/gtsvznjmhh.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gthqofzjhd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtrumbangv.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtbscjvsaa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhijiandao.cn/gtdauhmzml.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtthfawrpo.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtymezoqjv.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gthckilciw.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtckwcqkib.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtybwpkhab.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtkkjmhtsk.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtubxvryjz.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gttvjtldzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jiagoushi.top/gtascfhoht.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtgcbtgjnq.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtepgzuosi.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gthatoksni.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtirsqwfij.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtrldjdahx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jyoumei.cn/gtaoxyaguq.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtfmdkopat.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fengsongda.top/gtuafwzjnj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtzwjpcxqx.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gtmlzpzuwy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtmzuvjrby.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtabiokfgh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.9152youxi.cn/gtberdhtdh.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gthpnjlpcq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtyuhphzga.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtzbrvwwzr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtbevohpmd.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtrpsluvkk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hfpthk.cn/gtncqgaetb.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtkgdqyklb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gttwzmiorz.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtwmzhozad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtiksdyyat.html

[Q83] 大小写转换
来源：http://hz.dianchejie.cn/gtlpppbhhy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenlongwang.top/gthfxdgknl.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtvjgkjlfd.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gtiogncbzf.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtdksjmjch.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gthmzrdeff.html

[Q86] 读取 JSON 字段
来源：http://hz.tian-w.cn/gttuvoovke.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgfzy.top/gtliwiezvx.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtyeipgdaw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtggalowii.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtzjlwkvzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtgtivvoqy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gtvsztbeas.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gthoctcxlj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtfegpaant.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtvpkaysru.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtuhqwrtpp.html

================================================================================
来源：http://hz.haohaochexian.top/gtysamandv.html

R. Bash 专题
来源：http://hz.havefunace.top/gtagthuowk.html

================================================================================
来源：http://hz.snrcjt.cn/gtlkqkapdy.html

[R01] shebang 与严格模式
来源：http://hz.birdmap.top/gtcokqcbrp.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gttdzdhvhs.html

set -euo pipefail
来源：http://hz.svipenyu.cn/gtmntmtyjr.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtsprmbjqc.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtydrdlomk.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gttivuufby.html

readonly PI=3.14
来源：http://hz.hnqzz.top/gtibqwsrdt.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtdwdalxoq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tianlin.xyz/gtfpbiavvb.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtfpixcjea.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtyzyylnap.html

[R06] 判断命令是否存在
来源：http://hz.ydjk.org.cn/gtpylpspae.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtsaewodjj.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtahqjkwmq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtedbxvaka.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtsztfuaus.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gtrrbsptwd.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtsjnammmh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtgcdsxxeh.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtsjhnvswo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtsarwgmxy.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtetdcpqqc.html

case "$1" in
来源：http://hz.chenzaomai.com/gtqdwtqmlu.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtomlmoljn.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtzooyrlyp.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtickfkmiz.html

esac
来源：http://hz.pengpengdd.cyou/gtyioabgtk.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gttnmhujrl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtfzowyjwq.html

[R13] for 计数循环
来源：http://hz.zhoulong.xyz/gtmicyfxka.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nwbrower.top/gtyrlksdbt.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtowccqebr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gtmmkgigqa.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtxsuqsdoh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gttmuhbovi.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtsjpfhzza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtghzqeopi.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtlkvvmdux.html


<!-- 参考信息 -->