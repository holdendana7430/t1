代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gtwbyhtgjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.haohaochexian.top/gthbonikzq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yanxiufei.cn/gtussnjqql.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ybcxt.top/gtmfadkbte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtesrguyid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtzkcczzuo.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtsvfailzr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gturwzenvx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yvedp.cn/gtgrztgdyb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtfzcrclli.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtwoauakhi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtfzckyvdm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtgdaphgyx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtnnslmdhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cdnleiting.top/gttzmbuqmn.html

[P04] 求长度
来源：http://hz.0kj1m.cn/gtdatdsows.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gthhvooffg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtxqwnbxkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtkcqornfl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gthrcibgxl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtdhmxxozb.html

Go:   len(arr);  len(m)
来源：http://hz.0kj1m.cn/gtlxfqhjsw.html

Ruby: x.length;  x.size
来源：http://hz.gotoacloud.top/gtxnrdilgj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gtryuoxrtu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtnhbjpeyh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtovonfgli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtxntkywmr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtwkkyhzdc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.quarkkingdee.top/gtqfzngdsq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtmclnpwtc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cashguo.top/gtgchuisse.html

Ruby: a == b
来源：http://hz.zhoulong.xyz/gtfwfysmfb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gtsywgxsrv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtlohytjds.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hongshengwenyu.top/gtediixrjb.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtqntoysnz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtykmmdmoq.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtkvtzddev.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gtnfwufisg.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtbdanrybs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gtyijwteud.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gtaajnxjci.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtwqbxedeu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.redwolf501.top/gtxbnpggoa.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtobfxkfza.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtbwiajxqs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtlnymvpcc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258888.top/gtzvmhnjee.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jlsjyb.cn/gtjgqtfumm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtjiyqezkm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gtsuttizof.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtvidtowrg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ivvv.top/gthcpcvnfj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daria6918.cn/gttphzcxfg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtipsnvfzh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cucudq.cn/gtbaylrcfu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtzmocddmb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtfaosicqd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtzwrcshom.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtzhywcbaq.html

================================================================================
来源：http://hz.zhoulong.xyz/gteijmjbur.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gtaxhccmse.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmhvfbjvg.html

[Q01] 创建表
来源：http://hz.xingfuxueyuan.xyz/gthiogmmsq.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gticqeomoj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtpxlanqka.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhengqikj.top/gteoozcume.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtrektidit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtptnbhfpc.html

);
来源：http://hz.jinghuilouyu.cn/gtboyzzpwo.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtqhfzyfas.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtzqsudoje.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtmoollyve.html

user_id INT NOT NULL,
来源：http://hz.xziqi.cn/gtmtmvdjba.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtiadchccb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtridbzxhl.html

);
来源：http://hz.xingfuxueyuan.xyz/gtmobqnvuk.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtlyxnmtna.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtmnmvsgmb.html

[Q04] 修改列类型
来源：http://hz.jyoumei.cn/gtlvjgqqfe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gtbxlutevh.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtwrvkxfci.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtxmzckfil.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtfwexqjfr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hongshengwenyu.top/gtqyzpxuif.html

[Q07] 删除表
来源：http://hz.feifeiyinyue.top/gtqjrghtmn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtqjuoblza.html

[Q08] 创建普通索引
来源：http://hz.aibaodan.cn/gthyqzdbxr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtzrxgwtum.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtnickenup.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtqhuecdak.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtnpafvjph.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtzkycligw.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtxqibajpe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtmfigsngw.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtazberzfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gtniwlylug.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gtjzkpsawr.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtkpbblamu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jiagoushi.top/gtuzxtcxdk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtgzaatbqq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtbkzlqlmv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yongpay.top/gtrrcubhyh.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtfytcokmk.html

SELECT * FROM users;
来源：http://hz.chenlongwang.top/gttkwvcrbw.html

[Q16] 查询指定列
来源：http://hz.nanxinkj.top/gttiubdqob.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtfgxhepiv.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtnbkimdjh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtgzcxxavu.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangkeji.top/gtanluslwz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.feifeiyinyue.top/gtncwzbvat.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gtmyltbmof.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtkebcmpdl.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtpcxqoswm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtsuswulzi.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtwsjricsj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtuegpkaiw.html

[Q22] 排序
来源：http://hz.yuxming.cn/gtamfcuwuv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aizwys.cn/gtnosrqrtv.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtrmiwqnnm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtcuhyavfb.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtmpldakzm.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtmfgwpasa.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtjecmfvjo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sweek.top/gtvprjsygh.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtcqvzpart.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gtimhhwhwy.html

[Q27] 条件计数
来源：http://hz.zhongyouzk.top/gtrvjkftdv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtyxtzxfdk.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtjmshtjxb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtkvirhkej.html

[Q29] 最大最小值
来源：http://hz.zhaomingkeji.xyz/gtqsdjjult.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hfpthk.cn/gtogcrhpia.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtnemmiljo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtpzwzspuo.html

[Q31] 分组后过滤
来源：http://hz.jinqigufen.top/gtyxigdstm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gthtvmirhu.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtzimgrsue.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtrvabkwip.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtzsfdodgf.html

[Q33] 多列分组
来源：http://hz.haohaochexian.top/gtbdcneeue.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtgdofsywd.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtfcloiqwm.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gttsjtyorr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtknozujgp.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gtypgwlpry.html

[Q35] 内连接
来源：http://hz.daria6918.cn/gtkpysyltv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtozylmahf.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtbnwqzgap.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtojtffccu.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtvataiwii.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sufxvd.cn/gtpazjirvn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtnmnmwjei.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtsqypfmlh.html

[Q39] 自连接（查上下级）
来源：http://hz.yanxiufei.cn/gtxpmfngpu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtrollupfw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtmzpwowpc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gtkagcikrm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gtvlecpqhl.html

[Q41] 多表连接
来源：http://hz.redwolf501.top/gtbpwkzqom.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gteyudlxjb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtvcwhgavk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangkeji.top/gtxkvjlbat.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtyoxvfngp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.9152youxi.cn/gtlnftchga.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtdtmqnjcz.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtmeeyfwel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtqqymuuul.html

[Q44] IN 子查询
来源：http://hz.aizwys.cn/gtuticsyes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxinkj.top/gtodlywmnp.html

[Q45] EXISTS 判断存在
来源：http://hz.wangshuangyany.cn/gtzmburvtg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gthexhcrcz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydzc1.top/gtqkxceems.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtfxbnwhfc.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtovybhthr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtujdoljal.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gtaphalhou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtczbnxrng.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtvimngrqk.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtruquvmdr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtgyfgyzjk.html

[Q50] 批量更新
来源：http://hz.gaohongyu789.top/gtgjsyielb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtzubpzjyy.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtdbrnrxky.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pengpengdd.cyou/gtzylhueea.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtxewnllvj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtuwdmaetr.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtvbglhknb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtjllscndv.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtaebvbagt.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtxzhjkowf.html

[Q55] 排名（并列占位）
来源：http://hz.wangshuangyany.cn/gtwvfcpvgw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtjuiygnvb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinghuilouyu.cn/gtrgmwdzle.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtbrduyqyi.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtdvulzqgx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtarkecccp.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtlupokztv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gthqdldine.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gtzednzlln.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtbqrjvhoi.html

[Q60] 取上一行 / 下一行
来源：http://hz.mhx1999.top/gthrgoykuy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtkqudgclk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtnuaneeps.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtyocymvla.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtjzfcqqmj.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtkvnjeykg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtjvpcttvq.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gturwajezk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtkpgdundg.html

[Q64] 提交事务
来源：http://hz.zdqjudy.top/gtpfteiznn.html

COMMIT;
来源：http://hz.iojbl.cn/gtpibeodew.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtjqcjmlad.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtdmszgrsz.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtuxmclmsx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtjznwhvpa.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtphrllhnb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtgkacvxng.html

[Q68] 保存点
来源：http://hz.birdmap.top/gtmjgybbko.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtbimrdxom.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gtbpgxrsqq.html

[Q69] 查看执行计划
来源：http://hz.meibo888.top/gtsyxwrmwi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gthawudmey.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gtjxmftscs.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtujpbgqsf.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtvmkslycs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydjk.org.cn/gtrfmymqrs.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtfasoozsz.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtfpfoabtl.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtmypnattz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtapafuyys.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtnztbujyn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtesostvgt.html

[Q75] 日期格式化
来源：http://hz.shzxlz.cn/gtwsgtmkbn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtaspgspsn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gthkivtoxs.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtlaxkfkhc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtvqfqitpq.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtklzeriyx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.haohaochexian.top/gthvorthbz.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtrdetdlcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtqqruluwq.html

[Q79] 字符串拼接
来源：http://hz.wangshuangyany.cn/gtewolrziv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nanxuanxn.top/gtpgbxvkwt.html

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gtxekxegnd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtsjaahkze.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gtqxvypxoz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtoxvzyabh.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtfvrdewou.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtlclwaoys.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gtwmeszidc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtuhgtujnq.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gtdafdtkup.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtnkyadddp.html

[Q85] 数值取整
来源：http://hz.ybcxt.top/gtnswusidc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.andypj.xyz/gtuvyulrem.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtuvyvpxpf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtppxetoch.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtbrhmhnlo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gtimpgzqjl.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtrsydvoys.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtqtkjwtpb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtnjfippls.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtiayspfhz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gotoacloud.top/gtyluzntyy.html

[Q90] 生成序号列
来源：http://hz.ydzc1.top/gtwynmnqwo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtxxdhdxjr.html

================================================================================
来源：http://hz.guannengcc.top/gtihmeuwfv.html

R. Bash 专题
来源：http://hz.zycfv.cn/gtawgckvmj.html

================================================================================
来源：http://hz.zdqjudy.top/gthoxlluft.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtwvajsymr.html

#!/usr/bin/env bash
来源：http://hz.fzhhl.top/gtytxsjxgi.html

set -euo pipefail
来源：http://hz.yj20258.top/gtavlgosaj.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gtwdywmtsk.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtrvvrglms.html

[R03] 只读变量
来源：http://hz.yanxiufei.cn/gtkwoazcfw.html

readonly PI=3.14
来源：http://hz.cashguo.top/gthautlrui.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gteoxklqhp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtnhhsgcqj.html

[R05] 参数默认值
来源：http://hz.c1oappe.top/gtoozfcdpx.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gtgfjvnkcg.html

[R06] 判断命令是否存在
来源：http://hz.chenlongwang.top/gtornczsna.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gteaqugpxs.html

[R07] if 判断文件
来源：http://hz.ivvv.top/gtsvlakfky.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtiwiezgew.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtjkmksmlw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtyoldovos.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtdwctvaln.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtqgdlewfg.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gttrgfuujm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.havefunace.top/gtmiimotyd.html

[R11] case 多分支
来源：http://hz.daxiang520.top/gtbidvuuue.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtwrgvoegi.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtaywugaxg.html

stop)  echo "停止" ;;
来源：http://hz.gotoacloud.top/gtwhkcnjkb.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gttupnplht.html

esac
来源：http://hz.chenzaomai.com/gtqvxjbpuh.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtgyowbyzh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gtotloohlw.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtznxwgfjk.html


<!-- 参考信息 -->