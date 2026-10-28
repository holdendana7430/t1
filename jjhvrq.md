代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtkmbstwoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ybcxt.top/gtpmhhtpdo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtskuejzdt.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtnmewduxv.html

C#:   Parallel.For
来源：http://hz.mhx1999.top/gtdkfbxhgg.html

================================================================================
来源：http://hz.hywenlv.cn/gtugzlvuny.html

P. 常用工具函数
来源：http://hz.tian-w.cn/gtmynolowa.html

================================================================================
来源：http://hz.sweek.top/gtucsmefbm.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtjkspbrjn.html

Py:   str(uuid.uuid4())
来源：http://hz.wangdashe.top/gtjvvubgje.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtttedsgeg.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtvxwaqlsm.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtsadcmpxi.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtyunlgmas.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gtpowpwkrt.html

Ruby: SecureRandom.uuid
来源：http://hz.chenjidiqi.icu/gtkzkfdayq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtnsneasrz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yvedp.cn/gtehpgakrc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtgbfvmjbs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtfiysxlbf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yangfankeji.com/gtvestpfyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pycfn.com/gtwoqetzcb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gtnksebqko.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ivvv.top/gtjbfvpqhs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtzjyzlemh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jianghu66.top/gtqzwdspmg.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtfbfntwuv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtzihhsmdv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.iojbl.cn/gtnghpcepp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtidejxfok.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtuhdszsng.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gttxalavfe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtwmaayqnc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xingfuxueyuan.xyz/gttielqkic.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gtduvqlwcp.html

[P04] 求长度
来源：http://hz.jinghuilouyu.cn/gthvaxzebq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.bjfxy.top/gtccllccpu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gttubjregz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtfrixaxea.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtddalncid.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtwkteokho.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtxiggjfsu.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtgouysfdx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtxcucehgs.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gthwuvmdwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtwtscqgyq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtczswjaev.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtzbgupfrf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtfxvrwuhq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtgekwybsw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtevkhhpwf.html

Ruby: a == b
来源：http://hz.shanyushiyangtech.top/gtghcokzqg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258888.top/gtsvaqsqlu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtdhzcdmnn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gthwpucnch.html

PHP:  if (empty($x)) {}
来源：http://hz.zycfv.cn/gtplefegbw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtpcvnhypc.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtlnuythqc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.52xcode.cn/gtqvckjdlt.html

Go:   if x == nil {}
来源：http://hz.nwbrower.top/gtixcdhfxt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gthajcmdsd.html

C#:   if (x is null) {}
来源：http://hz.redwolf501.top/gtxartzddj.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtevkrobji.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gtjudlwtzo.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gteyipabnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtuekjgexu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtqcqeinvr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtoziqoyky.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtpwfjrmvg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtrlmekwsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtusiahlel.html

[P08] 处理浮点精度问题
来源：http://hz.cucudq.cn/gtabaczhvy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtkupfirim.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtbwddoqjs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.0kj1m.cn/gtmdeccdyu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daria6918.cn/gtveejirzz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtthseiuvr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xziqi.cn/gthwcbrwrc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtdknqktwx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtmnshmkoa.html

================================================================================
来源：http://hz.meibo888.top/gtbhuxwfnz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gtngkethqh.html

================================================================================
来源：http://hz.xylfe.cn/gtdcewcrwt.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtecanhrde.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtormiiqwj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtpecslakv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zycfv.cn/gtxvjqmnae.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tanke756.top/gtrqemlowh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtgqmvcvff.html

);
来源：http://hz.cheryme.top/gtinpvznne.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtmhaqfxnr.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtauceotqy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtihqoyczq.html

user_id INT NOT NULL,
来源：http://hz.nanxuanxn.top/gtvpkpkdpf.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtvmuaztoc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gtrbohahvy.html

);
来源：http://hz.jinyuanbaomall.cn/gtveqqxevh.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtengxqmpj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gttknrebsj.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtktnyklqq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtfnozjmue.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtjotdllko.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtlixhbobz.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtqmriaqkq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtaxadvzaf.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtphiaqsuj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtfjddqffp.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gteliddurx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gtrkhnfhiw.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtellvhwoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtbxtxuyau.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtnudsgclm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtbpptaclz.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtkzdtbphj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtojffmset.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gthnbareso.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtevdxomme.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnqzz.top/gtfigmoqpd.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtvzcfignn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.feifeiyinyue.top/gtsdzrkxnl.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gttqyipsgi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gtdylgqfzl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuetiantiany.cn/gtlqixgggy.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtzcmoowbh.html

SELECT * FROM users;
来源：http://hz.dianchejie.cn/gtifgbwyuh.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtbbinhevx.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtgsgluaiv.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtveyazdjr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtsgssaozp.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtujrsuwni.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dashuyun.cn/gtmrbmkgpl.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtwepnxzlg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtugiqnfow.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtxhpgcjcy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtacauejei.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtrviedzrd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtmpiaxprn.html

[Q22] 排序
来源：http://hz.havefunace.top/gtfnsegtmf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daria6918.cn/gttjabbfaa.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtticiwyps.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gtezyjgaqz.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gthdajhjmq.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtvqzfhtkq.html

[Q25] 只取前 N 条
来源：http://hz.gotoacloud.top/gtgdpaycnq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtbhhwpvpa.html

[Q26] 计数
来源：http://hz.fzhhl.top/gtivcvxnon.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gthcaphugm.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtngyvgxcw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuetiantiany.cn/gtyftdpazy.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gttavuuqmf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtxkmxojcs.html

[Q29] 最大最小值
来源：http://hz.pycfn.com/gtoktbqbyd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gtydnsjqhd.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtrflbbvuz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtusglosyh.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gttujbjqlb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtnnclhyxs.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gteajgjcom.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtsdslimhg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.feifeiyinyue.top/gtpggflesd.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gtoboigocm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtomrypkjk.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtuofwuylb.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtiayfbvgo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtewdyebrs.html

) t WHERE rn = 1;
来源：http://hz.hysaishi.cn/gtvzcnznpo.html

[Q35] 内连接
来源：http://hz.daria6918.cn/gtwexfuapa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtsxnnsksq.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtlrvjqqvd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtrjavbyrj.html

[Q37] 右连接
来源：http://hz.zdqjudy.top/gtkpldygom.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtpfhdvhpj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtjhvwfeqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtiigmlnqj.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtbktmbfav.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtmulwrzhs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gtpyderjmm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yangfankeji.com/gtzqldzglw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtnirozrtd.html

[Q41] 多表连接
来源：http://hz.hnqzz.top/gtjsbdnbiu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtsgrenevm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.wangdashe.top/gtcvdbryhz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydzc1.top/gtbetdvupv.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtwjmnodol.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtmvtqipyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ybcxt.top/gtubouegcq.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gthwhiqmbh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtzevzybte.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtvaldopfi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtnqjypnox.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtknjgwxup.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtayyozhsm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gaohongyu789.top/gtletbxwyc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtenjlynlu.html

[Q47] 与平均值比较
来源：http://hz.zhoulong.xyz/gtlmbjhamz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtopeyfvch.html

[Q48] CTE 公用表表达式
来源：http://hz.sufxvd.cn/gtxicgyutl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtvilmqgjp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gttxpucuph.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtrorhdpyr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtyqaxnjjw.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtzgcwlahy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gtscxajtfx.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtuqpqbnps.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.52xcode.cn/gthmyfyuxq.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtidwghuoh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cqqwz.cn/gtgqtevddf.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gthpngszne.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gthluohcwp.html

[Q54] 清空表
来源：http://hz.hongshengwenyu.top/gtmdsweuwb.html

TRUNCATE TABLE logs;
来源：http://hz.nanxinkj.top/gtzumawewy.html

[Q55] 排名（并列占位）
来源：http://hz.yangfankeji.com/gtyhreaqqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtpayncucp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtyztdnprk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtxcgivegb.html

[Q57] 行号
来源：http://hz.andypj.xyz/gtnolgsdok.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtfyqbyjsb.html

[Q58] 累计求和
来源：http://hz.jinghuilouyu.cn/gtljyuwlkk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sysykeji.top/gtrickjzti.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtzdmgpqns.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtyssgghys.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnxiangtu.top/gtifekakef.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yonumen.top/gtdijquwbe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jlsjyb.cn/gtfzadbvwp.html

[Q61] 移动平均
来源：http://hz.jinqigufen.top/gtptpsscuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtbqqrxggf.html

[Q62] 分组占比
来源：http://hz.xziqi.cn/gtxeoodyqa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtlpjjfemu.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtujbljylz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtrbdpugic.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtfsdivkse.html

COMMIT;
来源：http://hz.fengsongda.top/gtqmoliheb.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtgbboathi.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtzvigaggz.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtuhvylmep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtsgalxwzm.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtcgskgwie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtdvlbutej.html

[Q68] 保存点
来源：http://hz.shangyingyoupin.top/gtnafsieju.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtjwbsojup.html

ROLLBACK TO sp1;
来源：http://hz.yvedp.cn/gtufxtoxha.html

[Q69] 查看执行计划
来源：http://hz.mhx1999.top/gtwonmctps.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtmayftwkt.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gthutosuux.html

ANALYZE TABLE users;
来源：http://hz.sweek.top/gtsuyduxbl.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtgqglawbd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtdziwakjq.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gthryjjdka.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gteiogaubg.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtsbhnrakz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gttpeqdcqa.html

[Q74] 强制使用索引
来源：http://hz.tianlin.xyz/gtnosyslea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtemobtlkr.html

[Q75] 日期格式化
来源：http://hz.jlsjyb.cn/gtyudymqvp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yangfankeji.com/gtbwiugmas.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtsxffndsi.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtzpsxgzgp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtzgqecqiu.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtooxeokrh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gthjajdddo.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtcduhlcot.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtmswfapjq.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtqoficuqq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtfzttixgn.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gthlgvbxeb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtnrfdjfgc.html

[Q81] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gteydbedbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtsqvvvdad.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtaosremzm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtprjelved.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtcvdsakbp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtavuxunae.html

[Q84] 去除首尾空格
来源：http://hz.andypj.xyz/gtzehfkrbu.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gtsujvimnj.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtdwxwkqip.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtnxhfcmhw.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtvudejgyj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtxloutavq.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigfzy.top/gtgotoolbc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gttrrvekta.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgfzy.top/gttrbgcrhv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtzusfdpqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gttrutqbfb.html

[Q89] 判断表是否存在
来源：http://hz.smart0.xyz/gtadbkwfip.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtfmobazeg.html

[Q90] 生成序号列
来源：http://hz.yueranfly.top/gtcrxosach.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxuanxn.top/gtimakbbub.html

================================================================================
来源：http://hz.fzhhl.top/gtzgrscngg.html

R. Bash 专题
来源：http://hz.yueranfly.top/gtztwbvqjn.html

================================================================================
来源：http://hz.xylfe.cn/gtympcoyci.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtwqqdpvbq.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gthhgvhuob.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtiaqlgwfb.html

[R02] 变量赋值与使用
来源：http://hz.iojbl.cn/gtqosewfwk.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtkkgqylod.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtvkamzxrb.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gtfwuipzcd.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtcdqrnqwy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ppjwa.cn/gtafbyzcvh.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtmsgdkvsz.html


<!-- 参考信息 -->