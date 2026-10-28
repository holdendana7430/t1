代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtxuyhwtqe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtsvzvwzik.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtsrrmjllo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtdcyprskw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtqouespxv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtvzxtpzyo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtibkqyexu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhijiandao.cn/gtetimzibq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cashguo.top/gtjvhsmdpm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtotshppfi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ehwqpu.com/gtlzagnnzx.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtdvgufnso.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yanxiufei.cn/gtjjcfcngg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtqcrniljl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtjiaugkzo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtvaqdfwxu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtlymakuoq.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gtjghgcsuh.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtyyxfkvjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtayhcaxga.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtkjfrcylw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtudesepdo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xinyue.icu/gtqhttwcsf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sufxvd.cn/gtruvlkpys.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtmtnjknmd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gtsezzoakp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydjk.org.cn/gtnxxrzgrb.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtuygsqtdn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenjidiqi.icu/gtfkolydzg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtpgyyhcjz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtgxgfnjuz.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtndwfsasz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtrypeezxi.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtadnqzeuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtycbswuet.html

Go:   if x == nil {}
来源：http://hz.dashuyun.cn/gtrwcxgwcu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtavohuxxc.html

C#:   if (x is null) {}
来源：http://hz.gotoacloud.top/gtgkohgood.html

[P07] 防抖与节流
来源：http://hz.c1oappe.top/gthecbzvop.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258888.top/gtfdmfoibo.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtgpbkcbqy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtwiqifpxi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtkdnqdtfq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gteektfbva.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daxiang520.top/gtjnihayca.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daxiang520.top/gttznedkbt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuetiantiany.cn/gtxrvmpvdo.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtzejwczwa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtqpcyyspk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgfzy.top/gtaifpwpuh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gthkhxgjms.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtwpwslgwc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtstfcbpwd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtqnwxepgk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtjdpwoens.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zdqjudy.top/gtswmfxpug.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtofcjuqxv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuetiantiany.cn/gtbykcifax.html

================================================================================
来源：http://hz.zhengqikj.top/gtmoefmwxf.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gtdwlzzewy.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtduyxenel.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtayvxdcgv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtmulomkmv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtimlkomjz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtnlfhyloo.html

);
来源：http://hz.cqqwz.cn/gtqfyifoqi.html

[Q02] 创建带外键的表
来源：http://hz.hywenlv.cn/gtruncvvie.html

CREATE TABLE orders (
来源：http://hz.ywan-chungtsiang.top/gtfvofxmfz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtdokqlvri.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtbqbgzwlg.html

amount DECIMAL(10, 2),
来源：http://hz.zdqjudy.top/gtwgqjhogi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cheryme.top/gtcdvhixwt.html

);
来源：http://hz.cheryme.top/gtcsnwgtoa.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gttbvhtwuz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtyptbbnnm.html

[Q04] 修改列类型
来源：http://hz.chenlongwang.top/gttnkwktvd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hywenlv.cn/gtckmsiivj.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtdbbghlhy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtvjyfiwme.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtnjnghmpo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtlilljwqc.html

[Q07] 删除表
来源：http://hz.snrcjt.cn/gtifksvibk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tian-w.cn/gtongdpzyt.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtwbthzwae.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtfieuyqjh.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtqtlczpnl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtnkpitorg.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtkqgqkwmo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtzdyyzgtz.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtzmxprmur.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtdkbppcov.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtlaltfwjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cucudq.cn/gthcqtvzcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtuyxubnec.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtaesnqlln.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtzyjazhof.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtvrgbnzez.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gthndjprqx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtwyensfvq.html

[Q15] 查询全部
来源：http://hz.nanxinkj.top/gtcpmtgvtq.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtnxxhgxmm.html

[Q16] 查询指定列
来源：http://hz.zdqjudy.top/gteefemmwt.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtdlwuhpti.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtwgfocxry.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ybcxt.top/gtazgncrai.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtmpvddjyi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxinkj.top/gteayyrfiv.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gtwboubimv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtphbskxdj.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtnbcuetgm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxinkj.top/gtrohpfmox.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtcgumrjmi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gttuyqkqpc.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gttpctqybk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gtbufjhltz.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtochgluig.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtllovsitp.html

[Q24] 去重
来源：http://hz.cashguo.top/gtseccxpjh.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtqnfrhwlg.html

[Q25] 只取前 N 条
来源：http://hz.yj20258888.top/gtwzevxbqf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fzhhl.top/gtrognrjbm.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gthfyfwwph.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtgbepuyfr.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtjwbxxlnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtiayrcqvw.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtttnmhvgg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtbulhjlka.html

[Q29] 最大最小值
来源：http://hz.pengpengdd.cyou/gtdcnrkixg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gthkhbjibh.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtuckfmucw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gturhfvzmn.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtnscstuxf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aibaodan.cn/gtterktpxc.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtjelwpena.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtmzzurtvs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtzslymafz.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtljrpjjrw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shuidangran.top/gtplxihamt.html

[Q34] 每组取第一条
来源：http://hz.zhijiandao.cn/gtbzttsmbm.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtrixpnraj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtleikaqhd.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtjkhkouxy.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtawsspebc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gteiouvtel.html

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtgipjkpso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtmyuugrwo.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gteqhjcenq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gtamqpcocm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtzzyuhpnl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtuwekralm.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtduvcfkgl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtsykqgtyu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gteriaqjix.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yvedp.cn/gtnbnncreh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dianchejie.cn/gtxqmtokoc.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtjuvksyix.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenjidiqi.icu/gtfdamdblf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gturmehwgr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtejpuejjf.html

[Q42] 连接条件附加过滤
来源：http://hz.yonumen.top/gtcnzgapyq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtmcnsyxmx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydzc1.top/gtnkwxzdnd.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtjtxjsqup.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhongyouzk.top/gtxhmcyojb.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gttrmosigf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenzaomai.com/gtzrcdiuqd.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtoiilliqo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtmfuigxut.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtbeseisoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gthfgttogh.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gthwumzqva.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yueranfly.top/gttnvqgsni.html

[Q48] CTE 公用表表达式
来源：http://hz.yangfankeji.com/gtojvytdtb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtfdnaxsgt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtgodekfxo.html

[Q49] 更新单行
来源：http://hz.wangdashe.top/gtjhelukam.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtucirekmp.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtjkflqsgt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtvqurrmsn.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtbtfuoown.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtkaxmjzuq.html

[Q52] 删除指定行
来源：http://hz.sysykeji.top/gterzmoyrl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtpsonojye.html

[Q53] 按条件删除
来源：http://hz.iojbl.cn/gtsaljjlwn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhaomingkeji.xyz/gtkoelgfgg.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtxvdegxam.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtkqkqkjay.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtogulcnze.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtmdihzumv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gtguvfseja.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gthfzbgpyj.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtdwsfltpj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtzmmhvgaa.html

[Q58] 累计求和
来源：http://hz.bjfxy.top/gtbmarlqis.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtqwhijtfc.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtduvvfdqd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtfdwescns.html

[Q60] 取上一行 / 下一行
来源：http://hz.gogol.net.cn/gtspsnnbtt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtsqiaplbf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtaufxqwoq.html

[Q61] 移动平均
来源：http://hz.jyoumei.cn/gtiszlwbkc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtvvjdqhjw.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gttutbzlay.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtbgjstzwv.html

[Q63] 开启事务
来源：http://hz.tanke756.top/gtsycejbzr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gthjxgcsds.html

[Q64] 提交事务
来源：http://hz.gotoacloud.top/gtoydctlof.html

COMMIT;
来源：http://hz.bjfxy.top/gtfqogoblm.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtykjmkfgk.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtnnjaoipm.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtlrctevpg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gteuwkcmgv.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtrnicjlcv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cdnleiting.top/gtzqloswlm.html

[Q68] 保存点
来源：http://hz.jinqigfzy.top/gtfiaynfws.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gtxvfywdpe.html

ROLLBACK TO sp1;
来源：http://hz.zhengqikj.top/gtadtvwmkd.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtjzadtmct.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtmqnvislv.html

[Q70] 更新统计信息
来源：http://hz.hnxiangtu.top/gtxyxmwrre.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtloidhwyj.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtywyctkxt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtiewnenrc.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtqhfzuvef.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtlknhshue.html

[Q73] 查看表状态
来源：http://hz.hnxiangtu.top/gtuvzzfjau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cqqwz.cn/gtscehhdtp.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtjtqauudt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.quarkkingdee.top/gtnewdspek.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtuaivsavc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtzocedgtz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.meibo888.top/gtyqcjmyca.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtefrmptbw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtrsnpkkcj.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtoyilyhfk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtcqcrunut.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gtdsxcunwy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258.top/gtixqtmiib.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtlfpwkpcr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xingfuxueyuan.xyz/gteagibmkr.html

[Q80] 字符串截取
来源：http://hz.xuetiantiany.cn/gtawyffpey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gtudypnrhg.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtwpxlnwab.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtmxjclvmm.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtzaxeprvq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtgwpyhybf.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtvfbtsqrc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cqqwz.cn/gtdwezyabg.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtmjlsmcfe.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtytsnyzyp.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtstzyawfw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gthgeqvezh.html

[Q86] 读取 JSON 字段
来源：http://hz.zhongyouzk.top/gtecqxklkd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtdvshaatk.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtostldiih.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgufenzy.top/gtxjxxxfws.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtuvuydecg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtdgowopoe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jiagoushi.top/gteivstbhl.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gtaaxnywzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gtbevnylca.html

[Q90] 生成序号列
来源：http://hz.daria6918.cn/gtysedoxti.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtuhbowzcg.html

================================================================================
来源：http://hz.shzxlz.cn/gtemylbcxj.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtlbjndncu.html

================================================================================
来源：http://hz.zdqjudy.top/gtvzmtqfpg.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtzmagkatl.html

#!/usr/bin/env bash
来源：http://hz.quarkkingdee.top/gtzrzismxu.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gthhbpbvol.html

[R02] 变量赋值与使用
来源：http://hz.zhongyouzk.top/gtnltzdaxk.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtzuaylpwd.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtbdriledm.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtksxwntom.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtqpgvupvv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtyczdtpek.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtcoyezhmf.html

name="${1:-default}"
来源：http://hz.wangshuangyany.cn/gtghkqkojf.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtzujrhhum.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.andypj.xyz/gtpgakayhb.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtlqdgdtkr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hammf.cn/gtbrtjnvvu.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtsdpscwix.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtnevfcdtu.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtfcdjokct.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xingfuxueyuan.xyz/gtpbqnpkgz.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtsolmpbva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dianchejie.cn/gtukdkdisk.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtqlvidode.html

case "$1" in
来源：http://hz.jqgfzy.top/gttugeppkn.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtrqwnqcxd.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtrxpntajb.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gttjwnubor.html

esac
来源：http://hz.meibo888.top/gtqxbzvonf.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtukwbgwdt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gtysbaivcg.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtojuddcax.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtmzcnuxju.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtxujgochi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtpeqpybwv.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtxjledsax.html


<!-- 参考信息 -->