代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtycrrpnzv.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gtsvemfgkp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtkkayvpzt.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtxicdqwsn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtdtclridx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtfbjrpvmu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtwzkqulxn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gtzstiotbb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.redwolf501.top/gtgplnpuvm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtfoudtjqr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtphntpzqd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtfdbgjvtu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.iojbl.cn/gtlpiatizk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtrhiyqyei.html

[P03] 生成短随机字符串
来源：http://hz.tianlin.xyz/gtquhvnwax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sxryk.cn/gtqijtpcfd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtmtvyswfd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtwhhlrfuv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtvngsdzhi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtgcsdjblh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pycfn.com/gtzkprahdj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtijsmuarf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.kuanghao11.cn/gtpeavofcq.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtgbkbpikr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtejyjqumj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtruaumdlm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtjbfxczvc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtxoxjpvii.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jyoumei.cn/gtvcaciyoh.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtkzayvpde.html

Ruby: x.length;  x.size
来源：http://hz.bjfxy.top/gtgjswaoni.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangshuangyany.cn/gtqaeaguew.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtzslfbmak.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtlwigbovk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xziqi.cn/gtwzsryebt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtqwmjzdry.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gthblpylub.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.redwolf501.top/gtrzkmawzu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtryinsybt.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtvxdxctab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtlahuyzen.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangshuangyany.cn/gtdcaprlrx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gaohongyu789.top/gtjmzufzbg.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtcdssxbua.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtyslwmsyw.html

TS:   if (x == null) {}
来源：http://hz.vqdsnc.cn/gtylguiafu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.meibo888.top/gthdraluuv.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtxqguijem.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtfusgjnpc.html

C#:   if (x is null) {}
来源：http://hz.xylfe.cn/gtxrdzpgej.html

[P07] 防抖与节流
来源：http://hz.pengpengdd.cyou/gtgzlvectb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigfzy.top/gthuoxndpd.html

PHP:  // 手写时间戳比较
来源：http://hz.jianghu66.top/gtqyfpddzq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtkddjzdmi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtoclvibhr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxinkj.top/gtpmyjvqnb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtfskcjadw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtlgcmycss.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtonraxlup.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gthhmhrynm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtzbptqyvh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guannengcc.top/gtoejcgyei.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gogol.net.cn/gtnxgniqho.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtwxwnrlap.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangkeji.top/gtmnzivwlf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.0kj1m.cn/gtmibmmrtk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtjstogbco.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhijiandao.cn/gtggdlpjrz.html

================================================================================
来源：http://hz.snrcjt.cn/gtooeklxld.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gtwxywrypi.html

================================================================================
来源：http://hz.yuanzhike.top/gtswqmlnsy.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtmqtsznrv.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtxzbutkes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtbbdggonk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtgyfsjeuv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yvedp.cn/gthhhefdgy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.birdmap.top/gteytwnpmv.html

);
来源：http://hz.zhaomingkeji.xyz/gtjgeeynkd.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtepicxfuo.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtuadaslch.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtmdpgmwtt.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtkjrkdmds.html

amount DECIMAL(10, 2),
来源：http://hz.dianchejie.cn/gtsyvzwulp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtxpuqjpev.html

);
来源：http://hz.zhengqikj.top/gttwbjfjag.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtaxyfeejn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydjk.org.cn/gtllerdroa.html

[Q04] 修改列类型
来源：http://hz.yvedp.cn/gtsvietwqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gtniyfzyat.html

[Q05] 重命名列
来源：http://hz.yj20258.top/gtewwjukrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtxbjzdndu.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gtgxuxzczw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtccpnybme.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtgkvrfyvn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.0kj1m.cn/gtrefogrxk.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gtisajwgms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtfwhfhtpf.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtdgqirueu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gthlshaqun.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gtihzimjvw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gttcuufzxu.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtudrezyey.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cashguo.top/gtwkgluqvv.html

[Q12] 插入后取自增 ID
来源：http://hz.wangdashe.top/gtrchbiwkq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dianchejie.cn/gtjxoatkdj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtstfkenls.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtfekyvdpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ywan-chungtsiang.top/gttumwakwr.html

[Q14] 存在则更新（upsert）
来源：http://hz.smart0.xyz/gtzjzfpsug.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtmxnyahbr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtoexdyukc.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtrfqvjwqp.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtmrogxtkj.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtzsvvcryc.html

SELECT id, name FROM users;
来源：http://hz.zhiwuduotai.top/gtsmksjozb.html

[Q17] 条件查询
来源：http://hz.wangdashe.top/gtgulqsajk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtvmebfxcg.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gttxeimwco.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtomthciib.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtpgmxmhpv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtthxttawf.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gthvqwnuiu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydzc1.top/gtsinggcap.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtebrwylxb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gthrzeoxos.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gtecigczie.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pengpengdd.cyou/gtysyknjua.html

[Q23] 分页
来源：http://hz.sysykeji.top/gtlcjqyglz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gtahfllnyd.html

[Q24] 去重
来源：http://hz.jinqigfzy.top/gtrddbcwwe.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtdpayolpy.html

[Q25] 只取前 N 条
来源：http://hz.c1oappe.top/gtwqlkdcju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gtrkdrhvis.html

[Q26] 计数
来源：http://hz.jinqigufen.top/gtoxeexmph.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gtknnzmmcg.html

[Q27] 条件计数
来源：http://hz.tianlin.xyz/gtamfsxkdv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtqsgzbtuj.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtezlccrep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtehwtmyoj.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtjohsojhr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cashguo.top/gtsbuhvjhy.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtkyubmbae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtnyddeoqo.html

[Q31] 分组后过滤
来源：http://hz.cashguo.top/gthgzggllp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj20258.top/gtekayrihj.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtqmpqspsy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtmaqzpncc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtotccnoke.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtugjepwuy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xinyue.icu/gtyduknnds.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtmryzzrsr.html

SELECT * FROM (
来源：http://hz.tian-w.cn/gtqnonqofb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtnxgjvyzn.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtapybplaf.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gtbeobakmy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtgnlhsnmx.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gtdjvfyqhc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtfrrhsbeh.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtssqtitwe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtytohfpij.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cheryme.top/gtysuzqknf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtrtenfrrb.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtpfhxansz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtsmpbvxne.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtqqdmyguk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.bjfxy.top/gtpllputnn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xinyue.icu/gtgygvgjni.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtenhrncns.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtjljdnvbr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gtvaqbzejz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuanzhike.top/gtczvrocga.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtjktophdg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fzhhl.top/gtdzxszneu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtugixclmk.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtqgkmhwiu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtlqibdnst.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtcobwwyss.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtuzkntjoq.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtgcaknwjg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtwoapqmvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ywan-chungtsiang.top/gtfkegowvl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtejqnmevi.html

[Q47] 与平均值比较
来源：http://hz.dianchejie.cn/gtkkdqrlxq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtrqyvbzco.html

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtcdagklat.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtlicrlzsv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtkmuxutnx.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtgeqfbske.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtcwbtlpax.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtddbnzici.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtolnigyvx.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtdtlherik.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhixingplan.top/gtqiydmhfv.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtopzbqbxn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gthdvaixzo.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtucbeeftg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtbswereqd.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtpbwnedxe.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangtech.top/gtqxsxgghl.html

[Q55] 排名（并列占位）
来源：http://hz.tianlin.xyz/gtjuqypush.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sxryk.cn/gttaazqodq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnqzz.top/gtdnepzdhk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtqvnhlgkv.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtgljnalup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtijkeesll.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtnvmbdsym.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtjqvwgijv.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtkdpuurlf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtfwcmogxu.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258.top/gtimknzjsb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydjk.org.cn/gtjiceknvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtrklwqpep.html

[Q61] 移动平均
来源：http://hz.chenzaomai.com/gtyrrczigk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gtdnworuli.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtgxbdmibh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtidcbguoq.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtieqplvus.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dashuyun.cn/gtzzhrcoym.html

[Q64] 提交事务
来源：http://hz.zycfv.cn/gtopxuaspd.html

COMMIT;
来源：http://hz.xuetiantiany.cn/gtolncmpyt.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtjdpexmdy.html

ROLLBACK;
来源：http://hz.cheryme.top/gthiihogvn.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtbwczfqxp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenlongwang.top/gtxdhqjlqv.html

[Q67] 设置隔离级别
来源：http://hz.sufxvd.cn/gttghfwlik.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtvmpzuzao.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtptunqgeh.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtrxkakfwh.html

ROLLBACK TO sp1;
来源：http://hz.jianghu66.top/gtgwxiggem.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtjknbydky.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtybsvhvdn.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtilroswfe.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtydqxgvun.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gtgpkbffwk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.haohaochexian.top/gtvhnrcjtj.html

[Q72] 查看索引
来源：http://hz.aizwys.cn/gthsjkrvgj.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtnqalwetv.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtduyghbmx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gtxnihfame.html

[Q74] 强制使用索引
来源：http://hz.chenzaomai.com/gtyphycvjh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtqymsficb.html

[Q75] 日期格式化
来源：http://hz.smart0.xyz/gtlqhtezfj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtgvrofogl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtbpshmowt.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtlwvwzosd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xingfuxueyuan.xyz/gtpswpvwmf.html

[Q77] 时间加减
来源：http://hz.guowangkeji.top/gthxayxtzf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtxizwsxlb.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtmmijlozx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtfaetjmhp.html

[Q79] 字符串拼接
来源：http://hz.hongshengwenyu.top/gtawdtavcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtqdfxaeen.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtalkilbus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtrvatbovq.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtpaazkgeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gtmqngaxva.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtwyuzblqr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtnldqvgif.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtydlaigji.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ivvv.top/gtparotaoq.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtbshueouk.html

SELECT TRIM(name) FROM users;
来源：http://hz.yvedp.cn/gtdqurkeqf.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtgzyfjbns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenjidiqi.icu/gtbkaliozu.html

[Q86] 读取 JSON 字段
来源：http://hz.ydjk.org.cn/gtqrxihlvu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtdxuyzink.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtigwtrnwt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigufen.top/gtyxumukdz.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtulnntrdz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtzzqucvlk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.316326.xyz/gtwrviakln.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtlzbxojbg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.havefunace.top/gtfuuiwazn.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtenhpipug.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gtpkretljx.html

================================================================================
来源：http://hz.redwolf501.top/gtmjauowao.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtvwzbmavj.html

================================================================================
来源：http://hz.nanxinkj.top/gtigepbrub.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtukwmvury.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtrjzzgnwv.html

set -euo pipefail
来源：http://hz.gogol.net.cn/gtbsvpiidx.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtgsqgtgjg.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtjjirfmif.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtwfefkysg.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtikvyzivo.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtzntmzxts.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtypwrmbkx.html

[R05] 参数默认值
来源：http://hz.yj20258.top/gtcnndedwq.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtwquhqdhs.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtldrrutof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydjk.org.cn/gtybbucbnk.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtxgdgnfwn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtvmcivvsp.html

[R08] 数值比较
来源：http://hz.hywenlv.cn/gtqfiqzcah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtvbabmaww.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtqduwuhmt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtdpcbbzci.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gtqzgyfgkf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gthvaqejut.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtepbdkmuv.html


<!-- 参考信息 -->