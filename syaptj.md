代发 wailian999

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtxidjhrmh.html

================================================================================
来源：http://hz.yonumen.top/gtdszwradr.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtlpuplimj.html

================================================================================
来源：http://hz.cdnleiting.top/gtxtcrrfow.html

[P01] 生成 UUID
来源：http://hz.ppjwa.cn/gtiukufdef.html

Py:   str(uuid.uuid4())
来源：http://hz.ppjwa.cn/gtqbsrrqwm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtmpnsnpsv.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtzbmwdfst.html

TS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtsiqpfmjp.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtvxcxwlzf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gtzncduord.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtecejmgjh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtumvwlznl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.dashuyun.cn/gtbgmzyhhp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtjlqgmhzq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgufenzy.top/gtpanjlwsw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtllzsubsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtiulqtirf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gtnbopgwsv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gthvlhgrtu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtrwtuoiyq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shangyingyoupin.top/gtzuyopjqj.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gteetjxgcu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jianghu66.top/gtispgyqqy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtnvotqrbj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtuqfpnzjt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtziqzfvew.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gtjawoqagu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtjqqydqvo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gttgqvlzck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtpparcgmi.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gttwunigam.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtwarpcngg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtpehyawpy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtkzyhhqvv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gttucrreto.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtzhtdqlwd.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtskdksbdb.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtwuxnbboa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtlowfttqc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtkokqwogi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtslpuzgas.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtresnjdth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtmbzxxbpu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gtlqdfulrr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtxjulkdux.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtpdsnrfgd.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtkiiwqqky.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shuidangran.top/gtcflbzzse.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.svipenyu.cn/gtnzqtijti.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtqwbkkghl.html

PHP:  if (empty($x)) {}
来源：http://hz.guannengcc.top/gtxymvlwhh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtpxnyohvi.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtsknnvrdx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtrgqehxcy.html

Go:   if x == nil {}
来源：http://hz.gaohongyu789.top/gtrnwlrhvz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cqqwz.cn/gtmbeovjim.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtlkatwqxa.html

[P07] 防抖与节流
来源：http://hz.zhaomingkeji.xyz/gtbigycxog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtsipoferj.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtqlqvxcmn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtbxgvjjrd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtzjopaumv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtdzaaibsx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtzpskhinw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtnwqzhpdr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtvwmcnkbi.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtzhkmulga.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.iojbl.cn/gtolmkjubu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtvfcewvec.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtpbwcjlzg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sysykeji.top/gthvjfoauo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtyciehmqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhixingplan.top/gthhephnok.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ybcxt.top/gtixtlwxiw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hfpthk.cn/gtucpjbhgn.html

================================================================================
来源：http://hz.tanke756.top/gtjqletrmh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jyoumei.cn/gtlxuimmqt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtvnkwmvxb.html

[Q01] 创建表
来源：http://hz.yueranfly.top/gtxbvrqoqg.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtsnqgnmuh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtpjbhopys.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtblwzptga.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gzhubu.top/gtrtvvahas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtpigauytz.html

);
来源：http://hz.snrcjt.cn/gtqtizrlcq.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gtaiwdevlc.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gthguypizh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtnoibhrhc.html

user_id INT NOT NULL,
来源：http://hz.zhijiandao.cn/gtyhyefucr.html

amount DECIMAL(10, 2),
来源：http://hz.dianchejie.cn/gtmpnsrrdj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gtbftqlbjl.html

);
来源：http://hz.tian-w.cn/gtitmejfvq.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gtlpxbgpxa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yanxiufei.cn/gtnevhqeit.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtwnlwibdl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gttavrlpxk.html

[Q05] 重命名列
来源：http://hz.shuidangran.top/gtlrsbzeyc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtorcqtsba.html

[Q06] 删除列
来源：http://hz.yongpay.top/gtxhwihgto.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydzc1.top/gtzyaedhnv.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtydmigeon.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydzc1.top/gtifcqjfod.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtvlqjnivc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtyojywcnh.html

[Q09] 创建唯一索引
来源：http://hz.316326.xyz/gtzkuqflct.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtexlrtixt.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtslnretta.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.havefunace.top/gtkkdaslng.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gtbphlidaw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtlanwhahy.html

[Q12] 插入后取自增 ID
来源：http://hz.cashguo.top/gtczjbxglp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtbnbjalgt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtakwerjye.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtnfxzvcpf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtarzodfky.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gthkaxxrrr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xinyue.icu/gteltxyday.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtodxtsvze.html

[Q15] 查询全部
来源：http://hz.zhoulong.xyz/gtfidhehuz.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtohofqrve.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtaswdrvfp.html

SELECT id, name FROM users;
来源：http://hz.yvedp.cn/gtrhrqbbqd.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gteeabtpor.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ybcxt.top/gtjnftegml.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtisqzvvmt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtfvsgmjbc.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gtfbyfelvz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinyuanbaomall.cn/gtqvdyxlwf.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtiiexvxbq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtwnhptfzq.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtntatlkkg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtqpdjjtaq.html

[Q22] 排序
来源：http://hz.zycfv.cn/gttnaqazsv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nwbrower.top/gtskhahvsj.html

[Q23] 分页
来源：http://hz.snrcjt.cn/gtndheqykx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sufxvd.cn/gtyxnvmdps.html

[Q24] 去重
来源：http://hz.yj202588.top/gtgnvojvkp.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtshlrcvha.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtrcshjwth.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtfvsvigfv.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtdugzcjtb.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangdashe.top/gtxzcobajy.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gthmxorlnw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtzquphyhk.html

[Q28] 求和与平均
来源：http://hz.kuanghao11.cn/gtlqeumkaz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cqqwz.cn/gtcewoctjx.html

[Q29] 最大最小值
来源：http://hz.zhaomingkeji.xyz/gtrmrwznwt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtjauoixcf.html

[Q30] 分组统计
来源：http://hz.redwolf501.top/gtuyigvdkl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtpwsobmip.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtdayjppsl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jqgufenzy.top/gtlogkkpkq.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtgxsbggej.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtkymtedti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtjzoihlty.html

[Q33] 多列分组
来源：http://hz.yj20258.top/gtczwboyoy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gturwptuco.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtrqqoecdz.html

SELECT * FROM (
来源：http://hz.jyoumei.cn/gtdcwrymvw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtqxfzvlui.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtwodymhaq.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtwbjntqja.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtsikbpgop.html

[Q36] 左连接
来源：http://hz.jlsjyb.cn/gtngtkscoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtybouwbya.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtompxudju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jyoumei.cn/gtyzhpiekh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gzhubu.top/gtjbykxtta.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtqgdxccff.html

[Q39] 自连接（查上下级）
来源：http://hz.zhongyouzk.top/gtmehxtmoh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtdwzeucml.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gttrumrhgc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gtxmtzmpbn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.316326.xyz/gtajsnswrv.html

[Q41] 多表连接
来源：http://hz.xingfuxueyuan.xyz/gtydoqbbqb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtyhewmmys.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258.top/gtbpqrsnxd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtakiuhtpk.html

[Q42] 连接条件附加过滤
来源：http://hz.wangshuangyany.cn/gtewhxiaic.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258888.top/gtlolpzmpm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.snrcjt.cn/gtnmlrfdzq.html

[Q43] 标量子查询
来源：http://hz.pengpengdd.cyou/gtytqtjbuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtgmmgdmzn.html

[Q44] IN 子查询
来源：http://hz.jyoumei.cn/gtqgttavnt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.316326.xyz/gtpedqtvyt.html

[Q45] EXISTS 判断存在
来源：http://hz.iojbl.cn/gtbcdhdpku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtybjzokrf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtibzmnwqk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtpblhdphh.html

[Q47] 与平均值比较
来源：http://hz.jqgufenzy.top/gtlhsmrbde.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtjzgvotox.html

[Q48] CTE 公用表表达式
来源：http://hz.xuetiantiany.cn/gtlvpuepuw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cdnleiting.top/gtifguuhsu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gthkkmtqwl.html

[Q49] 更新单行
来源：http://hz.jlsjyb.cn/gtduevwxjs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtuiqeumhg.html

[Q50] 批量更新
来源：http://hz.cqqwz.cn/gtbbairhze.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ybcxt.top/gtxoqqtkbo.html

[Q51] 用子查询更新
来源：http://hz.yj20258888.top/gtgovwwfyk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.vqdsnc.cn/gtdkpemaso.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtnzoadddw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtolwpbycx.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gtbmhhpxuf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gtegmtlfcq.html

[Q54] 清空表
来源：http://hz.smart0.xyz/gtyoqxaxnw.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtwzpijiow.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gtltjioyms.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.316326.xyz/gtuumipjnv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gtenuwfogn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtjxhnudwa.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtdhahsgwb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.andypj.xyz/gtantgegfm.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtqcluqcmb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtfwpqgepp.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtqdehsuks.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtfqlunrru.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtxlmbhzcj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtuhrmnpgk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj202588.top/gtxymewoki.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtjajcrtpl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cqqwz.cn/gtrxlzclwj.html

[Q62] 分组占比
来源：http://hz.ywan-chungtsiang.top/gtsqhjfxth.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtwzuikpun.html

[Q63] 开启事务
来源：http://hz.cdnleiting.top/gttkdyxtkf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.mhx1999.top/gtpoefwnpw.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtzondddum.html

COMMIT;
来源：http://hz.shanyushiyangtech.top/gtpbfebpdb.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtereyhhgx.html

ROLLBACK;
来源：http://hz.yj202588.top/gtfletptyl.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtmxrilddr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtobfqknnc.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtckboapdx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuanzhike.top/gtpeotaiwz.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtbtncamvr.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtrejoivem.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtvjbimgmf.html

[Q69] 查看执行计划
来源：http://hz.nanxuanxn.top/gtrhmalgar.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jiagoushi.top/gtjkxotekx.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtllhpivjq.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtmtvqnavc.html

[Q71] 查看建表语句
来源：http://hz.52xcode.cn/gtdlyhhvyf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.birdmap.top/gtbfwtpnpq.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtafroeixw.html

SHOW INDEX FROM users;
来源：http://hz.zhoulong.xyz/gtjcgzihjf.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gttlfquuda.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtmbmbikzb.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gttdroutbl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258.top/gteewmrlih.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtvocdwunh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydjk.org.cn/gtsjjzbdux.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cdnleiting.top/gtwjjnefrv.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtrhmkipny.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtdiinypfp.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtqoqxeboh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtsofwapcw.html

[Q78] 当前时间
来源：http://hz.ydzc1.top/gtuyuveydy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtxkjssicm.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtlpmlwcxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtnwnhxcyq.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtgtgxexjl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gthmidqlhk.html

[Q81] 字符串替换
来源：http://hz.zycfv.cn/gtfdhpzjmd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gtgzokolwi.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtqhotzwgy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtmimtrbvt.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtwqooqqso.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtpkqozowz.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtkwxbltzp.html

SELECT TRIM(name) FROM users;
来源：http://hz.gogol.net.cn/gtjpxzydos.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtkywrlkzf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtvvdynoen.html

[Q86] 读取 JSON 字段
来源：http://hz.yangfankeji.com/gtsuepyvfz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gthyxpcnon.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtevriymkc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtcilauzmh.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtdaaeoyfs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtpwzanvsl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258888.top/gtoswxrmdk.html

[Q89] 判断表是否存在
来源：http://hz.gotoacloud.top/gtsfvzgjkw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuanzx.com/gteewjklfm.html

[Q90] 生成序号列
来源：http://hz.gotoacloud.top/gtvsaccmuz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.c1oappe.top/gtdctoimbw.html

================================================================================
来源：http://hz.nanxinkj.top/gtxnhpaaej.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtgaorghxd.html

================================================================================
来源：http://hz.cdnleiting.top/gtivkbxhfe.html

[R01] shebang 与严格模式
来源：http://hz.wangshuangyany.cn/gtvntxzgqm.html

#!/usr/bin/env bash
来源：http://hz.jqgfzy.top/gtqartkfmb.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtetoljwbd.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtlynhpjfq.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtnbepvwbf.html

[R03] 只读变量
来源：http://hz.chenjidiqi.icu/gtexcdsfth.html

readonly PI=3.14
来源：http://hz.shuidangran.top/gtpigpggex.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gtgroiarew.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtwaafgrob.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtnxhuasvr.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtpyubaxfg.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtyziyajgc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guannengcc.top/gtucrnjpbj.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtxxbycfzu.html


<!-- 参考信息 -->