代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtotyosmiq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtgdadvabh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gthavpphej.html

Ruby: // fork 块
来源：http://hz.cashguo.top/gtsheeifvb.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gtxmzlmdcp.html

================================================================================
来源：http://hz.xuanzx.com/gtctknobqe.html

P. 常用工具函数
来源：http://hz.jqgufenzy.top/gtneznkoik.html

================================================================================
来源：http://hz.svipenyu.cn/gtilnysqme.html

[P01] 生成 UUID
来源：http://hz.zhongyouzk.top/gtmicigutx.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gttnjnxgbp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtcrvizmtj.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtdkdzrpdn.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtzldwbkjd.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gttcejsaqq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtszsdmtva.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtcebdpaut.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gtxawkmsxt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtvoorftps.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtsynyduwj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtjcloskxk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hywenlv.cn/gtvrbxirso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtlgumftyb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.52xcode.cn/gthctiwobh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sufxvd.cn/gtfancqcux.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtxefjlrpq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hywenlv.cn/gtwwuomhmi.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtprpaqmyw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtkiptiofx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.birdmap.top/gtpetawpbi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtwmfjklal.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gthsisqnmx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhaomingkeji.xyz/gtvghcujfy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gttmaysoyv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtjiefcwjr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtzqnqjwww.html

[P04] 求长度
来源：http://hz.ybcxt.top/gtkaxfyack.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtwwgiwikw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gtanvzykqs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gttgszxrgp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtqqbqvxjm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangdashe.top/gtxsqmgnjf.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtotqgazlx.html

Ruby: x.length;  x.size
来源：http://hz.yanxiufei.cn/gtbbqvcjdu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.316326.xyz/gtkuzojbpz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtelccsmlm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtnhnodzcb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtwcrtqtzn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtxrfeebiz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtoaqhxerr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtyypsnxjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtoliweukn.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtjolqvoci.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hysaishi.cn/gtdrioeamw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtuzvhpovf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gtamdivyrr.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtvmfjqxqu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jyoumei.cn/gtsjyhyduy.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gtnufzcnin.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtljgmozgt.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtwlxibllg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtezwfgdtb.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtcdqvacku.html

[P07] 防抖与节流
来源：http://hz.9152youxi.cn/gtqhbvrwle.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gteaancwdi.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtpscqnluc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtykyoiwos.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtqbdvxpax.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258888.top/gtvkrlthcq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jlsjyb.cn/gttrhebbye.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtqccqppds.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtfcdxdlsf.html

[P08] 处理浮点精度问题
来源：http://hz.nanxuanxn.top/gtyttwwkon.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangkeji.top/gtovajhwks.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtrgspodtp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtnvohchbe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gthgnlcwpk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtqeaebere.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtletkjrsy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtfgistjbw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhaomingkeji.xyz/gtinlziyyl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvxgeiiav.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtodutsoba.html

================================================================================
来源：http://hz.cheryme.top/gtsgagwnht.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtrgwcwxgs.html

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtdkcwzzlb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtlsuuwnbi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtchqdktqm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtocnezkgv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtojnbmkwo.html

);
来源：http://hz.tian-w.cn/gtetqrgdru.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtofciizpx.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtpsthafby.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtuqrryoet.html

user_id INT NOT NULL,
来源：http://hz.yangfankeji.com/gthqomativ.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtpqvhjlcq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtkyzpvnts.html

);
来源：http://hz.zhengqikj.top/gtzppagmqj.html

[Q03] 增加列
来源：http://hz.jqgfzy.top/gtjqbvqoza.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tianlin.xyz/gtqwgpvqve.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gttwwihfiq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigfzy.top/gtyrmgkzfj.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gthcjijzwj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtfxnkzcew.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtgzdvlcsc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nwbrower.top/gtuswrqzqe.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtlecfpdvy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtavtjcdte.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gthqxbvxvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtqvgzanxu.html

[Q09] 创建唯一索引
来源：http://hz.316326.xyz/gtyudisoks.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtnccjuxfr.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtimsdrdoj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtrlfbayii.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtcvonpvfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hywenlv.cn/gtyschyffp.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtjxamnlpa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guowangkeji.top/gthcsiazro.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtbnncujal.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gthvlxzjkg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtbqythbil.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtinztolru.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtqyfmugch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtbalbcfse.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtmqunbqkm.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtlvijaluh.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtdwwbjpax.html

SELECT id, name FROM users;
来源：http://hz.chenjidiqi.icu/gtmzhpmvwg.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtahbnsrjz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnqzz.top/gtzuccevyc.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtunzjsfug.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtjhnsrddd.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gtxyypvdtl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtcumixqln.html

[Q20] IN 列表
来源：http://hz.hfpthk.cn/gtbcufuumn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuanzx.com/gtdndjmvhq.html

[Q21] 空值判断
来源：http://hz.tian-w.cn/gtudtswwnh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gthiakiape.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtouapiuph.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gaohongyu789.top/gtezdsxoxj.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtaduitvtt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtwmztxgpj.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtjliqnlnu.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtaivnozrg.html

[Q25] 只取前 N 条
来源：http://hz.yuxming.cn/gtiruttaqu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtlzkfffer.html

[Q26] 计数
来源：http://hz.jinyuanbaomall.cn/gtplvbjbvd.html

SELECT COUNT(*) FROM users;
来源：http://hz.tianlin.xyz/gtfupmlzxa.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtmohccqdl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhixingplan.top/gtczsoajcj.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtlwjgcoiw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gteaxootqh.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtvtvkpnvm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtrgzqxofr.html

[Q30] 分组统计
来源：http://hz.kuanghao11.cn/gtxgiymixt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtlqkeqnfo.html

[Q31] 分组后过滤
来源：http://hz.zhengqikj.top/gtfbatulhq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zdqjudy.top/gtwbwjovsj.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtndvjvgkt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtrjwcftov.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gtutvnckgf.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtlygsiaww.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtvlxsypwf.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtpaxyozsj.html

SELECT * FROM (
来源：http://hz.jqgfzy.top/gtnqyjsbnq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtyekedeiu.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtyuwlpebn.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtmbehndnb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtpznsdykv.html

[Q36] 左连接
来源：http://hz.wangdashe.top/gtxuyfqlml.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtupoiltvo.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gthoskvlaq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtydksqhnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cqqwz.cn/gtyltvclyj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.0kj1m.cn/gtgdpwuolu.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtbchzwnyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gtdyrnpvhy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtkvkqvrhu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtlaflwdhx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hammf.cn/gtkinayjvv.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtesadwwxg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.quarkkingdee.top/gtirgpvecf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhongyouzk.top/gtczjgydks.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgfzy.top/gtvuiavgwf.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gttzmxuxbl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtfjnzplwy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gthxkgoilk.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtnamolhsc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtrjpcuzrt.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtiggveycw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xingfuxueyuan.xyz/gtnrslcshe.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtzxjkymgw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtwjoepvvr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtimnaowsy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtzpcjbrbr.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtwetkbcvw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tianlin.xyz/gtxbxfgfef.html

[Q48] CTE 公用表表达式
来源：http://hz.kuanghao11.cn/gtryvkfrmw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtcepjpqzy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinyuanbaomall.cn/gtrbyeklsn.html

[Q49] 更新单行
来源：http://hz.shangyingyoupin.top/gtjtircqlp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtvveffmhi.html

[Q50] 批量更新
来源：http://hz.redwolf501.top/gtkgazuguj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtjyyhwjxj.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtwqdofuwd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtmgqjfktb.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtcbuibbwl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.meibo888.top/gtsrfsquze.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtjoxyjtgz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtvjpxidbj.html

[Q54] 清空表
来源：http://hz.yuxming.cn/gtfyfeodbw.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtqfsfhfgr.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtljlapryj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fzhhl.top/gtsppsasuy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gteeymylcc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtuxwlazlo.html

[Q57] 行号
来源：http://hz.jinyuanbaomall.cn/gtiiaxohnp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fzhhl.top/gtadxppggo.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtzakgdrkq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtljfvwxps.html

[Q59] 分组内累计
来源：http://hz.nanxuanxn.top/gtmyyhxiqu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtkmrbpmff.html

[Q60] 取上一行 / 下一行
来源：http://hz.bjfxy.top/gtxprpsrdd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtsneeclqw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtkfvqdhup.html

[Q61] 移动平均
来源：http://hz.316326.xyz/gtikscghtw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gtxybmlgml.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtkzacrgxx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtvnudsngo.html

[Q63] 开启事务
来源：http://hz.redwolf501.top/gttmgessch.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtwuctvzki.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gtuztlxpou.html

COMMIT;
来源：http://hz.yuxming.cn/gtvkkbclry.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtgjacjtbi.html

ROLLBACK;
来源：http://hz.meibo888.top/gtjztkgfol.html

[Q66] 行锁查询
来源：http://hz.vqdsnc.cn/gtzghwpomu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtrjkuntno.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gttgmghsqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gteklnuwsy.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtvazcmuao.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gttjlegjnz.html

ROLLBACK TO sp1;
来源：http://hz.fzhhl.top/gtlpvqpeuf.html

[Q69] 查看执行计划
来源：http://hz.yanxiufei.cn/gtwfwjhref.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtqzdjpupz.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtuowpzoxs.html

ANALYZE TABLE users;
来源：http://hz.zycfv.cn/gttwyajmxx.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtkbbygevp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtenvdalnn.html

[Q72] 查看索引
来源：http://hz.birdmap.top/gtguqipivn.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtenixwiin.html

[Q73] 查看表状态
来源：http://hz.zycfv.cn/gtdxuzjbxk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtwyaxkyvs.html

[Q74] 强制使用索引
来源：http://hz.meibo888.top/gtubsmmttf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtnkjkyvry.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtoscdtvaw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtfcybyjjm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtihhdwrma.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtowgojxss.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtzhyakjyo.html

[Q77] 时间加减
来源：http://hz.cdnleiting.top/gtnmslrnek.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ppjwa.cn/gtwbbtluii.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtsjvbxmoy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ppjwa.cn/gtwzhplayb.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gthnfdlllu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgufenzy.top/gtqzbnzksf.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtiumplxbj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gtdckkkidq.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtnjbyambo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtrznqkumy.html

[Q82] 字符长度与字节长度
来源：http://hz.yvedp.cn/gtsfkvknmd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gttxnqceoc.html

[Q83] 大小写转换
来源：http://hz.shzxlz.cn/gtkbqulxfy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtbqihdasq.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtjafxgcew.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtqmpxrtwd.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtwusaxvsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtnowxsvxk.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtdwawdirz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dashuyun.cn/gtihxfkrha.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtqiuyptru.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtnaessctn.html

[Q88] 行转列（条件聚合）
来源：http://hz.quarkkingdee.top/gtrbrijtkr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.9152youxi.cn/gtymqgvhhh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gtdmjsaaet.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtfptqyima.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shzxlz.cn/gtsfprsius.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtrmqtmnfv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtdbicygfs.html

================================================================================
来源：http://hz.guannengcc.top/gtmmvmtfbn.html

R. Bash 专题
来源：http://hz.fengsongda.top/gtmfqphioe.html

================================================================================
来源：http://hz.yueranfly.top/gthxbgtxmz.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtekmnpktk.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtqgeodbwq.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtqsghkacj.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtgtghrgzv.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtqjmvwaej.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gthxrvcaau.html

readonly PI=3.14
来源：http://hz.feifeiyinyue.top/gtsltyzqny.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtjrhmlkyz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtlmxvejzu.html

[R05] 参数默认值
来源：http://hz.yanxiufei.cn/gtginkkcuq.html


<!-- 参考信息 -->