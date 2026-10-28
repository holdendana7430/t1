代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtfkavcwvw.html

Java: UUID.randomUUID().toString()
来源：http://hz.kuanghao11.cn/gtsmceyseb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jiagoushi.top/gtxayokflj.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gthtscusye.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jqgfzy.top/gtrgmjslys.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gttetyodwe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtqktdhtrl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtecnkpfly.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dianchejie.cn/gtcibjpryj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gtmzmuhpzl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtobpwdlsk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sxryk.cn/gtdakmomci.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtfrpibchy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jyoumei.cn/gtqknlutcp.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtbtlhqthx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sysykeji.top/gtrzlwkggi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtsmwlxbix.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtboxnwbwg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtujgsbsad.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtmtcgqbud.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtvdkqtilp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shangyingyoupin.top/gtzgkaieqo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sysykeji.top/gtyefbkfzo.html

[P04] 求长度
来源：http://hz.gogol.net.cn/gtxiyzuefv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtxfwiykcn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtvewdmplp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtmslbpyny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtrlvpnuvd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtgnvojnir.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangkeji.top/gtkluswqpd.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangtech.top/gtdwjdmvop.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtpgqvwxzh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.316326.xyz/gtjfxyjtau.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigufen.top/gtiokyejfx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtsmnlehle.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtctuwtttm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydjk.org.cn/gtogjwdpks.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtyoptvkwa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangtech.top/gtrhgskwal.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtoaseowdb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtxgjuyxca.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yonumen.top/gtdajkxrfc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tian-w.cn/gtcevhzssd.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtujgvyhej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtiekfdyui.html

TS:   if (x == null) {}
来源：http://hz.0kj1m.cn/gtdpuaqupy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtrqowcgyl.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtpdqywjsd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtfyrrcede.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtygotqmfz.html

[P07] 防抖与节流
来源：http://hz.chenzaomai.com/gtumhlerhl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxuanxn.top/gtebabkmay.html

PHP:  // 手写时间戳比较
来源：http://hz.jlsjyb.cn/gthhpdgrdc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtfxusraee.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtuoifmhzi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xylfe.cn/gthqdgrwlw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ydzc1.top/gtafvbzghh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtsqvxulad.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daxiang520.top/gtqcthkqxa.html

[P08] 处理浮点精度问题
来源：http://hz.meibo888.top/gtgnmgtnqh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gtzsgqwcdd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhoulong.xyz/gtvydlhbpv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jyoumei.cn/gtkcworemg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtmgegxsph.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtdpyxurux.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtccgpzhkj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.9152youxi.cn/gtlygqmpes.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtiorgigpm.html

================================================================================
来源：http://hz.aibaodan.cn/gtasrhyduu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtlvvjynaz.html

================================================================================
来源：http://hz.sufxvd.cn/gtaupmutzf.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtcmrhgiak.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtododjvcz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtjeqcvkjt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.0kj1m.cn/gtotirzopf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gtrgeucfnc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtykhuzexw.html

);
来源：http://hz.fengsongda.top/gtachyawcc.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gtymgfbvel.html

CREATE TABLE orders (
来源：http://hz.hnqzz.top/gtvljcykmi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtcreasyvo.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtugptkxyo.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtpyzndgub.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydjk.org.cn/gtqzgotpwy.html

);
来源：http://hz.xuetiantiany.cn/gtssxhhekr.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtfhbuclrk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtxjtuspuj.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gtpdripjgg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtlmlvdkwa.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gthcltljqh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gtjkjztjim.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtmmznlmgu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxuanxn.top/gtdwcoeczh.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtvoilomoz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtkgezrkdp.html

[Q08] 创建普通索引
来源：http://hz.jiagoushi.top/gtanwskybj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.iojbl.cn/gtmhumgtwp.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtmqpdsaio.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtyqnvbnvl.html

[Q10] 插入单行
来源：http://hz.yuxming.cn/gtmmrrdosu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtclgmedmp.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtgugewobj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtkgobsprd.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtfjicxvia.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtixstaxin.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnxiangtu.top/gtihifxpcs.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gtfwqcyvgb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtwfwvfeqr.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtcmrownwj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtwzgsgoik.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gtitqmhhwf.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtvankvnxg.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtvdzgplkn.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtjhoxkrvc.html

SELECT id, name FROM users;
来源：http://hz.c1oappe.top/gtkzchdnjb.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtgbwexwtm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhoulong.xyz/gtxwvtbgja.html

[Q18] 模糊匹配
来源：http://hz.shzxlz.cn/gtxjjyuise.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yueranfly.top/gtbgheqgmf.html

[Q19] 范围查询
来源：http://hz.birdmap.top/gtunrhulpr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.52xcode.cn/gtgcbimhdq.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gteiuknatt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtfautknnd.html

[Q21] 空值判断
来源：http://hz.birdmap.top/gtcjwdekrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtduuayjfz.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtnoshcabk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtptfeicep.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gttgznyaeu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhiwuduotai.top/gtcbgumhnn.html

[Q24] 去重
来源：http://hz.sufxvd.cn/gtnjclnwhv.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtivnbmeoe.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtpkeelalh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gttrxfdifc.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gthivmqjdj.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtvlmoblja.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtrteiopeb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtginximsa.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtrgkinxex.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtufykrpag.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtzfzygjpa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zycfv.cn/gtwheozcpi.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gtgxxocpas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtgipqcdti.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtfqlzkcsu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gthzoaoupy.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtmtauxufa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtnqmgjiaa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtouonpmcm.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gthscytshy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gtvysxbyny.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtzqcdmlst.html

SELECT * FROM (
来源：http://hz.shangyingyoupin.top/gtffwyqkmp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinyuanbaomall.cn/gtptsemacc.html

) t WHERE rn = 1;
来源：http://hz.yonumen.top/gtjvobujxm.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gtybdsiyhc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtifqvnkzg.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtzamidtpp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtwnmutndy.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtpkzhlipm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhaomingkeji.xyz/gtoflfvceo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtbmquxalt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtylplyzmi.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtintorkoo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtorwbwtfj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtyopppbjb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtqztbpavi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.haohaochexian.top/gtwiwoqljo.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtibwiyubm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtztwuzhnp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtvvjrsdqm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtbqotntcp.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtxpqrrolr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtsrrmftmy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sweek.top/gtepowjlik.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtakxtnsay.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtqllpqkoz.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtkdsuvjws.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtsbxiqngd.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtbcepeqjq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtosefoczc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtiyffmzrb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtwdebjvpb.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gthaaqbfcd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtmkzupikl.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtkmcvkzxk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.havefunace.top/gtozqkdlyb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtrevpfpri.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtrvbmwtcd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtaecwdoii.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gtlxwqdzor.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xziqi.cn/gtmixbxidf.html

[Q51] 用子查询更新
来源：http://hz.ivvv.top/gtisppykmd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yvedp.cn/gtkrzbmwxg.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gtemibjacd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.9152youxi.cn/gtkjinrouk.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtaxcnihcj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtshntvjni.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtunxrajnj.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtpasrmggf.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangkeji.top/gtjhbuzpyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gthoosptfu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daria6918.cn/gtsdlqeblu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtuqydwqhi.html

[Q57] 行号
来源：http://hz.xuetiantiany.cn/gtzmhhwjtf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xinyue.icu/gtyrwrjcqc.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtiuqpvgio.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtfbioeuul.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtgizuumla.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daxiang520.top/gtwsrxqrux.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtjtveplin.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pycfn.com/gtfywhdnti.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtfighusyg.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtnlexlirf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtpyfebcge.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gthevrdjnq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtzboppolt.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtkowgsiwh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtndgvvflm.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtxeiwihlq.html

COMMIT;
来源：http://hz.zhongyouzk.top/gtwyvduzep.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtshxcotxa.html

ROLLBACK;
来源：http://hz.yueranfly.top/gtvnbunhkh.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gtgjmtbncv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gttfsoqjju.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtgjjvzuev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtaenvoxpm.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gthgjdubsm.html

SAVEPOINT sp1;
来源：http://hz.svipenyu.cn/gthaknyhdk.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtogkicfpn.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtvcryxefq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtfzmmjfmt.html

[Q70] 更新统计信息
来源：http://hz.shangyingyoupin.top/gtefxsuget.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtxyphjbcn.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtaaxpjcok.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhiwuduotai.top/gtoitydinf.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtyftwnakd.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtasaznfux.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtywtdtrbj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gthmsekvwt.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtvfjzhbwv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hfpthk.cn/gtnlseotaa.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtcxzwjrzn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.quarkkingdee.top/gtwipjoywz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shangyingyoupin.top/gttlwgotxw.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtfffmyury.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yonumen.top/gtvgqueexp.html

[Q77] 时间加减
来源：http://hz.cashguo.top/gtgcbekala.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtkyrjxjku.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtvurzihob.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtwatfdaoz.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtqjmmiqjz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtlktafvat.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtoaidundq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gtouqkxoht.html

[Q81] 字符串替换
来源：http://hz.ydjk.org.cn/gtzwktmbep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtriqgzbtz.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gttqblnjse.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtmejqufhq.html

[Q83] 大小写转换
来源：http://hz.52xcode.cn/gtcxbswiij.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtzwsazwhi.html

[Q84] 去除首尾空格
来源：http://hz.jinyuanbaomall.cn/gtburthqbc.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtvrpqorhe.html

[Q85] 数值取整
来源：http://hz.meibo888.top/gtcusjvwtm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtzhhyjsie.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtyqgcnyvm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtslpcbpjv.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtqqsoqehe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnqzz.top/gttcepbmfo.html

[Q88] 行转列（条件聚合）
来源：http://hz.sxryk.cn/gtrekhcnkn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtieejfnbt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gtokqlrelu.html

[Q89] 判断表是否存在
来源：http://hz.xinyue.icu/gttlhwfjxp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtiuxvaric.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtrchicxme.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtccumzhle.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwwhdazaz.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtwmdkptvp.html

================================================================================
来源：http://hz.yuanzhike.top/gtsppzepjf.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtqzjqyazm.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtolyyaqyp.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtvoiwkssk.html

[R02] 变量赋值与使用
来源：http://hz.shangyingyoupin.top/gtaohqqved.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtgigvqgvp.html

[R03] 只读变量
来源：http://hz.nwbrower.top/gtuziwgllh.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtkxccjtpf.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtgfimpifh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtjueutvxn.html

[R05] 参数默认值
来源：http://hz.chenlongwang.top/gtbkadnrsw.html

name="${1:-default}"
来源：http://hz.ivvv.top/gtnbuachga.html

[R06] 判断命令是否存在
来源：http://hz.pycfn.com/gthkiqrpyj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yongpay.top/gtthviztwa.html

[R07] if 判断文件
来源：http://hz.tian-w.cn/gtlogrlegu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtrlkjzyaz.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtnytcfaea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxinkj.top/gtorngdfrp.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtxwnifqkg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtsvqjfvdg.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gtenkmowts.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenjidiqi.icu/gtbfuvtpzh.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtzcyomcda.html


<!-- 参考信息 -->