代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtwfyfpkpf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.0kj1m.cn/gtgvypqmey.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtkhdgkset.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.bjfxy.top/gtmzngvslp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtnwkjfyqc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtpbmyxzfc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtqzwjwudx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jyoumei.cn/gtpawpatzh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtqckzcrfx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuxming.cn/gtrahcjrov.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aibaodan.cn/gtvvhuoqlv.html

[P04] 求长度
来源：http://hz.yuanzhike.top/gthzwbdegm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cdnleiting.top/gtiwdwkjrx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtiygjpmks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtrtsxqjdi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gthchfblng.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenlongwang.top/gtnntwbtkh.html

Go:   len(arr);  len(m)
来源：http://hz.zhongyouzk.top/gtetjjsaas.html

Ruby: x.length;  x.size
来源：http://hz.sufxvd.cn/gtuwqsgtgl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jiagoushi.top/gtnpwaunwy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shzxlz.cn/gtfwnebwtr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydjk.org.cn/gtugnyynlu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtysawhdrx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinyuanbaomall.cn/gtdzahmkuf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtdvihamsm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenjidiqi.icu/gtgjekxadi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gotoacloud.top/gtdnzerxmb.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtnrzloqee.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtudfyrnbp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtggtruuqw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtkfaixhzh.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gtcazjhyma.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hywenlv.cn/gtzybtzela.html

TS:   if (x == null) {}
来源：http://hz.ywan-chungtsiang.top/gtjhmukooj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gthodlusos.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtmtlmnvmm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tian-w.cn/gtxzblaibo.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtpguznjqu.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtslnnwzmz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.aizwys.cn/gtyvepfmbd.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gtltuskqyu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtvtloqeel.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtxvevettc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigufen.top/gtovfhxcqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yonumen.top/gtfoyunxhw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hongshengwenyu.top/gtkcfdrqcu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtwphvoyns.html

[P08] 处理浮点精度问题
来源：http://hz.nanxinkj.top/gttghhycjf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtmcwljkoc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtvtdirbaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtktdisnlr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.havefunace.top/gtqzryyxuj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gtrdthnswc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtkblnmlxg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daria6918.cn/gteffjikru.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtotznaufs.html

================================================================================
来源：http://hz.xinyue.icu/gtvqacswdr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gtoeyqnncs.html

================================================================================
来源：http://hz.xziqi.cn/gthubfsise.html

[Q01] 创建表
来源：http://hz.xuetiantiany.cn/gtxomvxumq.html

CREATE TABLE users (
来源：http://hz.zhaomingkeji.xyz/gttbfsxfdi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtjehoymbc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gthadgxiwz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gtqcctvziq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtfltkecys.html

);
来源：http://hz.yj20258.top/gtdlgehtxq.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gttmdjsrqn.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtbwiftwgg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtcigvbhgr.html

user_id INT NOT NULL,
来源：http://hz.zhijiandao.cn/gtnbjwrqln.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtjqjytqst.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fengsongda.top/gtdcbyiytb.html

);
来源：http://hz.zycfv.cn/gtjoxaemxz.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gtwxzdneuk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xylfe.cn/gtijdhypmm.html

[Q04] 修改列类型
来源：http://hz.zhaomingkeji.xyz/gtginvnljt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gtxvmvetkd.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtcahdbcsr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtifmilhvf.html

[Q06] 删除列
来源：http://hz.sxryk.cn/gtdlfvnezj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtnwgbzbrh.html

[Q07] 删除表
来源：http://hz.zhoulong.xyz/gtaljczrdp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.snrcjt.cn/gtppaztzph.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtbxwmffel.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtvuqajpmo.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtyfpgonjy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shzxlz.cn/gteezlhxdt.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtztaewpqi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtupcszgtz.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtdojrzmwi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtbxdmfafw.html

[Q12] 插入后取自增 ID
来源：http://hz.haohaochexian.top/gtafqgnayg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtlunbswxd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtvvuswsiy.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtsenyqiaj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtzfkrqfum.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtegrknhul.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtmdwvvqgh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.quarkkingdee.top/gtuykzjjer.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtkusrmfuq.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtlihxibii.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtnhtscjis.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtkhecxkbr.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtqoiozwuq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gthzcawgrs.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtjmbxvjck.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtkleqwzlt.html

[Q19] 范围查询
来源：http://hz.52xcode.cn/gtfxczcbpr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtbbtgrhne.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gttdvkzcmh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtadywvqvw.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtcnbhvbcg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtddtdlsrd.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtxhvwiade.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.mhx1999.top/gtutudbkpd.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtxfeiqaiy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtdtmphlpk.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtybmkxweq.html

SELECT DISTINCT city FROM users;
来源：http://hz.kuanghao11.cn/gtftuierfq.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtsixtqyqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj202588.top/gtlxwldscg.html

[Q26] 计数
来源：http://hz.jinqigufen.top/gtvnwjeieg.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtnylpltwk.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtxnmzluif.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jiagoushi.top/gteepzanrx.html

[Q28] 求和与平均
来源：http://hz.feifeiyinyue.top/gtkiwtlhpp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtmcupqtnh.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtwdhxoxie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtfxuzlznc.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtryiytyqa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtcdnzykto.html

[Q31] 分组后过滤
来源：http://hz.pengpengdd.cyou/gtfdiqnigk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yvedp.cn/gtunsyeksf.html

[Q32] 分组拼接字符串
来源：http://hz.hongshengwenyu.top/gtvcsxvqey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtfhcqfilx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtnmrybqkf.html

[Q33] 多列分组
来源：http://hz.jqgufenzy.top/gtgnsmwvoe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtdqsmyljn.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gtrqojdmre.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gtoxkxnydi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangshuangyany.cn/gtutrigiio.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gtozmdtkmy.html

[Q35] 内连接
来源：http://hz.aibaodan.cn/gtdkcywebl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gthglyffce.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtvpxzgtrr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtiyvqxtou.html

[Q37] 右连接
来源：http://hz.shangyingyoupin.top/gtmstgrvuv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gtpkfgwxeg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gtekpfrhmr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtahuzesiy.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtczasmwyk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtjjsxwgke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gtkdrhfvwj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.svipenyu.cn/gtcoxcbuaz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtgqsbvqel.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtemhzyupl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gthtzhtnsv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gtdxvtetha.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtoxlrynzb.html

[Q42] 连接条件附加过滤
来源：http://hz.iojbl.cn/gtxvdkkxev.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtdmlvvkpc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtemrimuyr.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtyfeznggg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtktlkgnwh.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtduirjgmw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gogol.net.cn/gtrsjxsiew.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigfzy.top/gtxsvnwsnb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtqehuenve.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenzaomai.com/gtbngrflna.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtzkjdfhjc.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtqwrqutni.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhongyouzk.top/gtyadlglbo.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtcqfsczmy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yangfankeji.com/gtzozuhlid.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtpefpuijs.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtezfropmz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtzovqplkk.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtnbhosylg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtekjqdedu.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtkgkhxxda.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtreqbrpyv.html

[Q52] 删除指定行
来源：http://hz.0kj1m.cn/gtudgmihme.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtuhnepggd.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtsbzeaqew.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.kuanghao11.cn/gtrhvbotjt.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtnkqcgpiv.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gthpfnejwk.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtorsvddxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenzaomai.com/gtojphdbpl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtblwstpoq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gtcahlzsyw.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtgnizjwnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtdzqyualx.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gttsywktzm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.c1oappe.top/gtbjneejnv.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtjbdqvzot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gtevmsusvg.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtugqskwxm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gtcasfdpss.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtmpzvtxok.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gticvybtxj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.meibo888.top/gthrywvler.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gttosbxfdt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtjmksefht.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gtdmkeoruv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.9152youxi.cn/gtkbgrjswh.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtfxluaygm.html

COMMIT;
来源：http://hz.sysykeji.top/gtvgldzthc.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gtlwtocybp.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gtyzikoyei.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtzbaauzvl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtnxosmpcd.html

[Q67] 设置隔离级别
来源：http://hz.daxiang520.top/gtdrjsauxc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtjcxdpdrx.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtdkrhdrwt.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtvhvefvwc.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtcvrvkxyp.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtqkupypmx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtbgbsurqa.html

[Q70] 更新统计信息
来源：http://hz.dianchejie.cn/gtndzqxwxu.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtcrkgzffr.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gtdqfeoqmc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtzibthasr.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gthykejhms.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvfhsezcf.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtzzjpgdze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtgahiwbht.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gthirprhul.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtwocvxfol.html

[Q75] 日期格式化
来源：http://hz.pycfn.com/gtygzcimka.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtesoqtnxy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtvrouognr.html

[Q76] 按天统计
来源：http://hz.hnxiangtu.top/gtszvkagty.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtucfifdku.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gtootghyld.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtnotphtif.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtfzqfetaf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuetiantiany.cn/gthwlfdbbh.html

[Q79] 字符串拼接
来源：http://hz.snrcjt.cn/gtpdmpumbf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtajluymvv.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtvydxtexl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtkzfowlrf.html

[Q81] 字符串替换
来源：http://hz.zhijiandao.cn/gtplmxlfsd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtopavxwzz.html

[Q82] 字符长度与字节长度
来源：http://hz.vqdsnc.cn/gtjancuiuf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nwbrower.top/gtrvlgkniu.html

[Q83] 大小写转换
来源：http://hz.zycfv.cn/gtuusipchn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtcthvpkai.html

[Q84] 去除首尾空格
来源：http://hz.redwolf501.top/gtwyhiemba.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtmivacbuw.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtrcqapthj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtcypfcges.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtyeyasaro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtsozxtmbb.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtyqqlnbbt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuxming.cn/gtkmhmihnp.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtpsuecoco.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtcyxgdcud.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtjdjmdlns.html

[Q89] 判断表是否存在
来源：http://hz.andypj.xyz/gtfshlpyqk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258888.top/gtgavothyh.html

[Q90] 生成序号列
来源：http://hz.cucudq.cn/gttbpwhskm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.smart0.xyz/gtxlvkrlit.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtiswngtyw.html

R. Bash 专题
来源：http://hz.xuanzx.com/gthqxbbcml.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkaegrdrz.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtrxjdbvco.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtuoiqiwek.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtimasrkli.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtfpeodhzq.html

name="Tom"; echo "$name"
来源：http://hz.xingfuxueyuan.xyz/gtdkpakktg.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gteucradmz.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtalfmzwze.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtrltcipyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hfpthk.cn/gtskwextbx.html

[R05] 参数默认值
来源：http://hz.havefunace.top/gtkeekkhke.html

name="${1:-default}"
来源：http://hz.cdnleiting.top/gtonudolla.html

[R06] 判断命令是否存在
来源：http://hz.jinqigufen.top/gtiygypwei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtvmdvqkpr.html

[R07] if 判断文件
来源：http://hz.havefunace.top/gtmmmbuloi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ybcxt.top/gtjiklqcga.html

[R08] 数值比较
来源：http://hz.52xcode.cn/gtefcocpyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtmgjgbppf.html

[R09] 字符串比较
来源：http://hz.yangfankeji.com/gtfdrnjofv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtsjnfumww.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtzwzitjgc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.c1oappe.top/gtkzqnvnzn.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtsokgspfp.html

case "$1" in
来源：http://hz.shanyushiyangkeji.top/gtxeetpypr.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gthanrtuit.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtxqcawzfq.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtlneznagc.html

esac
来源：http://hz.zhengqikj.top/gtsyiqorvr.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtjgfboxtk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtquwrppbr.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtdulauxzu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhiwuduotai.top/gtldoiqcyu.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gtnennpgph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fzhhl.top/gtcazbngrp.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtjryxmoux.html


<!-- 参考信息 -->