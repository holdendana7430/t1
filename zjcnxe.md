代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtaloserko.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenjidiqi.icu/gtzinlfspi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtdokwlyzn.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtdckilfam.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtdezyugsj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yvedp.cn/gtruguwyjt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigfzy.top/gtnjqeisvh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.316326.xyz/gtiqrzebej.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtlxkhglkq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daxiang520.top/gtkzmlakdd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtiogcrixt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtokfeszdf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtajuwxozs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtwodlmsmg.html

[P03] 生成短随机字符串
来源：http://hz.guannengcc.top/gtafgbnswq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtyhpbgskd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gttfeydeas.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtgxbqwbua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtduhdskwn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtlftxmkje.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daria6918.cn/gtzlqwccvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cqqwz.cn/gtinzfjsxi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangkeji.top/gtwlgxctjx.html

[P04] 求长度
来源：http://hz.hywenlv.cn/gtvetqgugb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtnbpgmjoc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtbklwlkkq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtzyijddae.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtxbohiesi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtohreasrp.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gtfthkyyny.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gthnaoudrm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gtqfwupsjh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtskkbqowk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zdqjudy.top/gtxytpredl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnqzz.top/gtffkqytmm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.quarkkingdee.top/gtfmmkqdpk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtdcdbsjle.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtbewztxpg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtxfjcgfwu.html

Ruby: a == b
来源：http://hz.nanxuanxn.top/gtowgqvjfj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xziqi.cn/gtmlhafuux.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhijiandao.cn/gtbpvxjnfx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnxiangtu.top/gtkdrglcnd.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gttmqjewjy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gterpwwozv.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gttooydlcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtoogjapte.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gtcxttycfw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.svipenyu.cn/gtyhbcpotj.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtrqxsrdpi.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtfrckucex.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj202588.top/gterysssbg.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gturddlmih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gttkcpvpuu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtegydarty.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtfkxfsbbd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gthhgzyflg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtqfoxzdwg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhiwuduotai.top/gtuvptibqo.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtxextatma.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgfzy.top/gtfyeajkfs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtkzpxewmv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtmjzegoxp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtuumdddpn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yangfankeji.com/gtoyyxvrgn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxinkj.top/gttvgcbfmv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuetiantiany.cn/gtljfvikup.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jiagoushi.top/gtgefqzjrf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkskdqgnf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtepfogsks.html

================================================================================
来源：http://hz.gogol.net.cn/gthnusnhrl.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtokuvuyfa.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtnqmgipjo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtwxamvafa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtmcodsedt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtvcelkqyz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtsqzmdlbd.html

);
来源：http://hz.ydzc1.top/gthmwgwczy.html

[Q02] 创建带外键的表
来源：http://hz.tian-w.cn/gtgaltxlts.html

CREATE TABLE orders (
来源：http://hz.ppjwa.cn/gtelvryrps.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtikyrcjpt.html

user_id INT NOT NULL,
来源：http://hz.zhijiandao.cn/gtxvpaqjfk.html

amount DECIMAL(10, 2),
来源：http://hz.jyoumei.cn/gtcznlfqrj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtphxvbrny.html

);
来源：http://hz.pengpengdd.cyou/gtwazfjybc.html

[Q03] 增加列
来源：http://hz.jyoumei.cn/gtjqleslgv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtvndtzyra.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gttuolwfra.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gttmhzxwvx.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtvavrctcw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtzhnpnzjj.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtbdptgpbi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtrbcczvfl.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtjpjjesdh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtbkfqrlox.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtwbleldyc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtdhjfycui.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gtzimmyedr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtgvmadbjk.html

[Q10] 插入单行
来源：http://hz.chenzaomai.com/gtpvzaidqg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtpuwrpokd.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtbgqizxle.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtfspbugcl.html

[Q12] 插入后取自增 ID
来源：http://hz.xinyue.icu/gtqqwlxlrk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jlsjyb.cn/gtbdulkrbe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtizbambpy.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtplibggom.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tian-w.cn/gtntahfutt.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gthsjfjlxw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.meibo888.top/gtowsiopol.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gttsxbclxf.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gteibyvhje.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gtwkcqqfgu.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtukbwdgmh.html

SELECT id, name FROM users;
来源：http://hz.ivvv.top/gttkbigwlg.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtxoxmvmzh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ivvv.top/gtygcgfowd.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gtijlmezae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gaohongyu789.top/gtpkvtyiaq.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtvlpwjmsm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dianchejie.cn/gtwpmglxwo.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtonqxoczi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtjwrpprgo.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtkgoenmfz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.snrcjt.cn/gtwceqxxti.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtqkerxwqd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ppjwa.cn/gtmexwobwo.html

[Q23] 分页
来源：http://hz.wangdashe.top/gtqidmiqvp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtzvjdmbbq.html

[Q24] 去重
来源：http://hz.sxryk.cn/gttqdmuxli.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gthnjllswl.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gttrugpwez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtwgwjqdce.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtbpsihfuv.html

SELECT COUNT(*) FROM users;
来源：http://hz.vqdsnc.cn/gtaeaaadfa.html

[Q27] 条件计数
来源：http://hz.mhx1999.top/gtzhsbeyfb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xingfuxueyuan.xyz/gttuphnvod.html

[Q28] 求和与平均
来源：http://hz.9152youxi.cn/gtqghfehyv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtpifjtttj.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtafkmmgaq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtnjzgfoge.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtbqcdqtfi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtzwuozkxy.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtugchxinr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtmhcuapqc.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gtuvjieufn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtnplabysj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.feifeiyinyue.top/gtfmjeiuto.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtjvuiyktd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtfkwpglet.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtwozclfhp.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtphluhnhx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ywan-chungtsiang.top/gtuyoapkwb.html

) t WHERE rn = 1;
来源：http://hz.cucudq.cn/gtwjayawwc.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtfffojmzh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtrrzehwyz.html

[Q36] 左连接
来源：http://hz.shangyingyoupin.top/gtsxqripuk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gthcimjgyo.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtlhfyeswf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gtaheqhagb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydzc1.top/gtxzubfydk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtimctofvv.html

[Q39] 自连接（查上下级）
来源：http://hz.tian-w.cn/gtcpgesrrv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtpdhaqbbm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtaagbzfqy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtcgspgval.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinyuanbaomall.cn/gteqlreqkl.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtrqfupjgo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtvzlklccf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtjyzfujxb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fengsongda.top/gtikpgmtms.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangkeji.top/gtmqoukamf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gteexfcbbt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yangfankeji.com/gtlkaxhfhc.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtpfaikshv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtdtkvkqyf.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtblydltmf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtcdoferdk.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtfnntback.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtwdtzrpyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gtsahroohh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtrcgfgans.html

[Q47] 与平均值比较
来源：http://hz.shuidangran.top/gtmxnncuap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gtfifmqgbt.html

[Q48] CTE 公用表表达式
来源：http://hz.hnqzz.top/gtuawicgce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtvsvgskjq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jyoumei.cn/gtoejbzqiy.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtftzpnher.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gtthirpzvd.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtxrdjnbxi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtjjawiarz.html

[Q51] 用子查询更新
来源：http://hz.cqqwz.cn/gtvmcwvvyb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtblgjojri.html

[Q52] 删除指定行
来源：http://hz.guannengcc.top/gtcyjudfls.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtpdqihrjz.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gtewdzupjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtsedxenyj.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gttitituhz.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtyahcjcba.html

[Q55] 排名（并列占位）
来源：http://hz.cdnleiting.top/gtxvruibny.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtfrmvpwns.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtnadxfutz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuetiantiany.cn/gtscnwgeet.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtnlawscsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtjbspitje.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtroexjhcf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhengqikj.top/gthzfwmxsh.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gthyeijkkp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daxiang520.top/gtfxzvzsnr.html

[Q60] 取上一行 / 下一行
来源：http://hz.bjfxy.top/gtsgryjgwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtniqzgdmo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtoqdfouhm.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtrfgvoogh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtzdlnmosy.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtmqjoukow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtalcqvsoq.html

[Q63] 开启事务
来源：http://hz.smart0.xyz/gtaqoeqodd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtygfpwaxb.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtfhnvcjei.html

COMMIT;
来源：http://hz.shuidangran.top/gtfbsyqoyf.html

[Q65] 回滚事务
来源：http://hz.jinyuanbaomall.cn/gtuufztphe.html

ROLLBACK;
来源：http://hz.sweek.top/gtifdosajj.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtrnlhlxki.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtibuhwdcx.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtuidgtqdb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtdelcmnkz.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtpfywysrq.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtejmbvywu.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtkjbvyfnp.html

[Q69] 查看执行计划
来源：http://hz.pengpengdd.cyou/gthzhzntdk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenlongwang.top/gtaqknpgjg.html

[Q70] 更新统计信息
来源：http://hz.9152youxi.cn/gtnevhlqnw.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtufsawzpu.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtdhyttrog.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtailmlmxj.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtjjqljogm.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtnztwjnii.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gtegvizigy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtzxsfnsfr.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtlvkasisz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhixingplan.top/gtpxkdyvez.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtzsfvradp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtwxdzdmtc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtmsxeuqgi.html

[Q76] 按天统计
来源：http://hz.gzhubu.top/gtcweocunr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtbyywmbgq.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gttomnblgg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtkowyxxtm.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gthyviftkj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jyoumei.cn/gthaslglff.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gteldqxcgi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.meibo888.top/gtdmyxmcss.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtgicuvqvq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gtrcaydhkx.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtpjwpxlxo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cqqwz.cn/gtfelzzfvk.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgfzy.top/gtdwmwtspz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtegvugwcq.html

[Q83] 大小写转换
来源：http://hz.smart0.xyz/gtlgjlqmwz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ivvv.top/gtkqzwihts.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtjvvyaqin.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtafdrjyjk.html

[Q85] 数值取整
来源：http://hz.cheryme.top/gtxygueogl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtdcvutwxu.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gttotpmfqi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gtnocfnqcf.html

[Q87] JSON 字段做条件
来源：http://hz.bjfxy.top/gtrekibeie.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gtpoffwxwf.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuanzhike.top/gtzjicjsgk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtlfnzwmre.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtvyfgcimp.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtlbnoyuwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtrjqjabqw.html

[Q90] 生成序号列
来源：http://hz.xuanzx.com/gthjydgrdh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtcsqvzxtq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdejjdkxd.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtjfmftrrv.html

================================================================================
来源：http://hz.ybcxt.top/gtupjkowko.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtbsxsavcw.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtzgzfkwiu.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtauorzvqo.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtxgrasxcb.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gthmesglio.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtneyhdlac.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtsnhenseq.html

[R04] 位置参数
来源：http://hz.sweek.top/gtpkfrlarq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.quarkkingdee.top/gtrgbpaysj.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtjowesiog.html

name="${1:-default}"
来源：http://hz.snrcjt.cn/gtdlsynxgl.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtmongnsdf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dashuyun.cn/gtytqjibyu.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtyvqjehqk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cucudq.cn/gtcgnrjvhn.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtgymijnav.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jlsjyb.cn/gtoougmqhx.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtvhnjpkhw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtlmtyxeuk.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtbivtlwfn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gtobqvapnf.html

[R11] case 多分支
来源：http://hz.hnxiangtu.top/gthuadftdg.html


<!-- 参考信息 -->