代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fzhhl.top/gtdscforfq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.smart0.xyz/gtfuxtwbnz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gtwmmxlhfa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gtmvqbisqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtjywrcoga.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gttrdnrblw.html

[P03] 生成短随机字符串
来源：http://hz.jianghu66.top/gtihkszjpk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gtlmfpepmb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtvuassaiv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtacoyazhq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtqbqyhjun.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gthqnfnsml.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aizwys.cn/gtotyzlcbi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sysykeji.top/gtfxxbhysd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtywskcplc.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtevbkqubx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.vqdsnc.cn/gtaugraefg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtfunffavx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtgraktnfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtutoapaym.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtmnpxxwrs.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtewnyxmli.html

Ruby: x.length;  x.size
来源：http://hz.sweek.top/gtftbzakzw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtlhpkgmsc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shuidangran.top/gtangjlqnt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigfzy.top/gtuzadxwjh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dashuyun.cn/gtxqcpuodn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtpwbnceta.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtwyegftvd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj202588.top/gtvpdpnpsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigfzy.top/gtkpngranm.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtrguwwffm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gtvsgjppsl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jlsjyb.cn/gttkhptjqz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtvqploikp.html

PHP:  if (empty($x)) {}
来源：http://hz.yanxiufei.cn/gtjdukndzd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shuidangran.top/gtckyyqizk.html

TS:   if (x == null) {}
来源：http://hz.redwolf501.top/gtjhsimqkj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtgysnbmba.html

Go:   if x == nil {}
来源：http://hz.xinyue.icu/gthreolpxi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtwmowlsxx.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gtceakhphn.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtjetktjhv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydjk.org.cn/gtdjovjpqx.html

PHP:  // 手写时间戳比较
来源：http://hz.ivvv.top/gtisnzipuy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gttjgmqzrm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtdluhjfvo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtgjisiqwr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.vqdsnc.cn/gtxvxftpcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guannengcc.top/gtwdknqeso.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtlloizvhn.html

[P08] 处理浮点精度问题
来源：http://hz.cqqwz.cn/gteqhmrbil.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtvljzqbcf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtswcwslqt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtvdqylrbz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gtvlfubdin.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.9152youxi.cn/gtugphyfjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtirdtfavw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gthlcogcyd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtdqwjgmvn.html

================================================================================
来源：http://hz.gogol.net.cn/gtgduktcnw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtzjgrjjca.html

================================================================================
来源：http://hz.0kj1m.cn/gtuovoqjwh.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gtdktgphgw.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtpiipgjce.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtbnfgmkwk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gthbtliziu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtmkofwaan.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtdpkzbriq.html

);
来源：http://hz.ywan-chungtsiang.top/gtqsmqoeqf.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtuaxwxzee.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gtbafurorz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtzhtyoogr.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtykidrbqa.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtrgizzfov.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhoulong.xyz/gtvfufwgfp.html

);
来源：http://hz.birdmap.top/gtgvkwtcvb.html

[Q03] 增加列
来源：http://hz.jinqigufen.top/gtsaencfom.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtzzjmoqzr.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtuovvpgfe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtnrinumfr.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtngewntcs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtexdviwwx.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gttvcwjlsl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xinyue.icu/gtrokxnhjq.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtuymvrqvv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxuanxn.top/gtnzpxsbmi.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtdkaeyway.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtbptjggef.html

[Q09] 创建唯一索引
来源：http://hz.wangdashe.top/gtakdzvlft.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtihdkugau.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtmilmihjo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gotoacloud.top/gtamdizcmd.html

[Q11] 一次插入多行
来源：http://hz.sxryk.cn/gtvqvdmbgv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtpadsyjop.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtmhwnmsaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ehwqpu.com/gtgwqlgdzp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtqptrvkrq.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtehowqfom.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hongshengwenyu.top/gthylagvvx.html

[Q14] 存在则更新（upsert）
来源：http://hz.gotoacloud.top/gtpnqrqucl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtuexmggkn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtuvnffwmc.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtixyvzfmq.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtlzlfadyl.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtkgslzikn.html

SELECT id, name FROM users;
来源：http://hz.xziqi.cn/gtaovpmyct.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtageeriut.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gaohongyu789.top/gtbrkxfhzx.html

[Q18] 模糊匹配
来源：http://hz.haohaochexian.top/gtowmyjktq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gaohongyu789.top/gturgulbjz.html

[Q19] 范围查询
来源：http://hz.aibaodan.cn/gtvdfkbjnn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtbcrzlwxk.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtxseudroa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.0kj1m.cn/gtppghblct.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtcnaazwni.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tanke756.top/gtsjaywoxj.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtmzwhyknx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shzxlz.cn/gthidigvci.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gttabgwlru.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtpdeqohwx.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtstacighd.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtnwqgkwnk.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtowgklrvz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gtusgsbtwg.html

[Q26] 计数
来源：http://hz.jyoumei.cn/gtoajnxirn.html

SELECT COUNT(*) FROM users;
来源：http://hz.snrcjt.cn/gtlkxnwuvw.html

[Q27] 条件计数
来源：http://hz.hnqzz.top/gtdhymcroh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtlvdykckc.html

[Q28] 求和与平均
来源：http://hz.zhijiandao.cn/gtyfniiuee.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtezogfjjr.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gteaechwbg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtemnybdrx.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gtyedxldri.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtqoknedol.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtjopocbzv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tianlin.xyz/gtljbrgzzn.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtcewijpgn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtearzaehz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xylfe.cn/gtloxygzhv.html

[Q33] 多列分组
来源：http://hz.iojbl.cn/gtjdedvpce.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtubskojux.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtgouhjfqa.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gthmmmjtac.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hfpthk.cn/gtruxwtfzl.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtcvqzaeoc.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtcburpemk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtekeqqbhi.html

[Q36] 左连接
来源：http://hz.yj202588.top/gthaapeyji.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtpnlbirdj.html

[Q37] 右连接
来源：http://hz.hammf.cn/gtpjbhxpcg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhaomingkeji.xyz/gtcbnxdsjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnxiangtu.top/gtgqbvqelo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtdbqtduux.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gthepunyin.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jiagoushi.top/gtydfbqvec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtczpojsnr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtrwsfttrs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gtrjuennfb.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtsdjyxubx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtouxexdbn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtlfwkmcgr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtqvnzarva.html

[Q42] 连接条件附加过滤
来源：http://hz.zdqjudy.top/gtpidjkaph.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtdkygfofp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtfviqnvjd.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtqxsljypp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtuejjbudc.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gttyavllcg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ppjwa.cn/gtveokolvu.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtpknebzpj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtkqcbuxup.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuanzhike.top/gtdinouqxu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtvvvsibmz.html

[Q47] 与平均值比较
来源：http://hz.zhixingplan.top/gttzzzwfkq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtfztnpdrj.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gthslymooi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtmjbwuoct.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yanxiufei.cn/gtxkzrjhtl.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtkohabfap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtebdjuecy.html

[Q50] 批量更新
来源：http://hz.yangfankeji.com/gtbkbfulfd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangtech.top/gtdlkgxnqe.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtoqtapfuk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtiiqkrcjy.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtfzkszeyn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jyoumei.cn/gtftpvnnyg.html

[Q53] 按条件删除
来源：http://hz.ywan-chungtsiang.top/gtptyotqid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtgkftayxh.html

[Q54] 清空表
来源：http://hz.hammf.cn/gthikpmwpe.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gtmrvaejjd.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtpvcdnajm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gthpfxxaeh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtwswvevzl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtgdiotqbd.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtymrurldp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtouzpcaaw.html

[Q58] 累计求和
来源：http://hz.cdnleiting.top/gttlmbegfs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xinyue.icu/gtlqfqwrsf.html

[Q59] 分组内累计
来源：http://hz.zdqjudy.top/gtunqofpcf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtokihjzgh.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtzelbapho.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtiiozibkb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtcexugjoc.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtgbinnuau.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtzmhahepo.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtneedmzph.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtkprkjqmi.html

[Q63] 开启事务
来源：http://hz.nwbrower.top/gtxghilube.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydjk.org.cn/gthwfkbmvx.html

[Q64] 提交事务
来源：http://hz.guannengcc.top/gtkbztwulj.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtugjekhse.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gteaxvcbtp.html

ROLLBACK;
来源：http://hz.bjfxy.top/gtcxazgyeg.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtbifewdue.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtgavpzmjc.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtqkqeownl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.0kj1m.cn/gtphjtsszu.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtgjvetjvn.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gtqstwggwd.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtomnfgayh.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtvmoqvuax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gthabevijv.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtjyzlctdi.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gtisbdamkv.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtujbtwylm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jianghu66.top/gtjkrbepqp.html

[Q72] 查看索引
来源：http://hz.hongshengwenyu.top/gtebtxvshx.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtchuskomr.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtphadygoo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtojdmoxbq.html

[Q74] 强制使用索引
来源：http://hz.shangyingyoupin.top/gtfcxpbqxb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gotoacloud.top/gtawowcrvu.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtqvjnogkq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gtwgoiphmp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gttgomigpt.html

[Q76] 按天统计
来源：http://hz.meibo888.top/gtzpgnywga.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtuvjxptoe.html

[Q77] 时间加减
来源：http://hz.birdmap.top/gtgufjppia.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.52xcode.cn/gtvgsolkvy.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtzjuzwqqx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtcpgbfvny.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtidprxpjs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtdpjithqt.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtnxryvkbe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtgoevtlvw.html

[Q81] 字符串替换
来源：http://hz.chenzaomai.com/gtjpqoqlmu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sweek.top/gtxeylpzzx.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtfajmrnqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.kuanghao11.cn/gtnqitylur.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtrdghqhpo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtbwwevqev.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtviowdedp.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtacznpnai.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtmpovyeem.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtamdexhgi.html

[Q86] 读取 JSON 字段
来源：http://hz.xuetiantiany.cn/gtunvjvfuj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gtybfymfiv.html

[Q87] JSON 字段做条件
来源：http://hz.9152youxi.cn/gtxpnnkcab.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.9152youxi.cn/gtxmcogsgg.html

[Q88] 行转列（条件聚合）
来源：http://hz.cashguo.top/gtyxzhaxfj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gtujkzswxl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtmckksbmp.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtkoyaygua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtzizijsah.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtcvkazizw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yongpay.top/gtrjwouloj.html

================================================================================
来源：http://hz.kuanghao11.cn/gteafsmobl.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtfsmlljyr.html

================================================================================
来源：http://hz.gotoacloud.top/gtrxgiedfx.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtywtxaety.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gttkgjirzv.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gthjgsscra.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtheabnyas.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtghpquepb.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtvfwfjiix.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gticpbajoq.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtxeqmbvfp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtgdiqjero.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtupgnlfsa.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtskzvilnv.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtrusknvrm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gtoxunhvme.html

[R07] if 判断文件
来源：http://hz.kuanghao11.cn/gtbkrixyxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gttjllreyg.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtyoswasgx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtoftlrqkz.html

[R09] 字符串比较
来源：http://hz.yangfankeji.com/gtnhkuzrdc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtiuzjdajo.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtjfaaoytz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtnbusdvyc.html

[R11] case 多分支
来源：http://hz.svipenyu.cn/gtkpfibnpy.html

case "$1" in
来源：http://hz.chenzaomai.com/gtafeyrjfo.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gtwnegmdbc.html

stop)  echo "停止" ;;
来源：http://hz.meibo888.top/gthsqrpihk.html

*)     echo "未知命令" ;;
来源：http://hz.hfpthk.cn/gtodbrrxdt.html

esac
来源：http://hz.nanxinkj.top/gtsinluryk.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gtlolztoqn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtjaxgqzgi.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtplhqlvmu.html


<!-- 参考信息 -->