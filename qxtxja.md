代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtwbfwmvfm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtxtwgngsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gotoacloud.top/gtdkxhjtqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gturgzoltv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtqludpyln.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.mhx1999.top/gtbshgdwsl.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtevpmiurb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtsgqdsykk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtxpgxqygp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtahjgvoht.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtpibbmnls.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtpiyhlzyv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.316326.xyz/gtclxdfieg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gttcptxzyd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gtbbcrorzf.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtzjrpltir.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gttphhbxwf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtttovrbhf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtfgdpgimq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gterrqzjkn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtasvpofon.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtjwvsqfoz.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gttipfnbqk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtrorlgmmb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtaqsjezth.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fengsongda.top/gtvxttdruz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtqdqaukfy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhaomingkeji.xyz/gtbecmmvgj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtskxuuogh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtfpjhcusw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtxfmtvhie.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gteusdptqw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtvckqjbfe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nwbrower.top/gtchvxlapc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtiqoydcsn.html

PHP:  if (empty($x)) {}
来源：http://hz.fzhhl.top/gtmkqkkjzg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtvfttrcfq.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtddtimhyd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.meibo888.top/gtbmjhmntw.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtillcyxdc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cucudq.cn/gtljmwfiww.html

C#:   if (x is null) {}
来源：http://hz.zhongyouzk.top/gtifyavgih.html

[P07] 防抖与节流
来源：http://hz.zhiwuduotai.top/gtinyyqpmc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtmjcdaqof.html

PHP:  // 手写时间戳比较
来源：http://hz.ivvv.top/gtkznmhpcc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtdmxlhikb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtffodywzx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gtawuzczhe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gthwskhgwb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gthrowetae.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangtech.top/gtzhcvlirt.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gtqrpjupha.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtvmaaondi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtwzwoteip.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtazrlvuyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtdqdnfnht.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gteqfwgeyw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtjzstpyux.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gttrocpvgj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtqrfzzurw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbeyowdga.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtdabhbmob.html

================================================================================
来源：http://hz.yj202588.top/gtlfgatfus.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtrjgcjlxg.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtxszftuow.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtnyskhsyp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gtapxkoudu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtenjziyyo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtzlvoputp.html

);
来源：http://hz.guowangkeji.top/gtorfssimh.html

[Q02] 创建带外键的表
来源：http://hz.ybcxt.top/gtcoxrrlsb.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtnqymfiax.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtyzaxbukt.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtglmxrxcy.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtvixoslbf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtdriyhrwe.html

);
来源：http://hz.yanxiufei.cn/gtdwtgnhww.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtfecihgrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gtekdnpyyv.html

[Q04] 修改列类型
来源：http://hz.jinghuilouyu.cn/gtuszpflrq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gthvbgnfmd.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gtipouwjhj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gthnhejgei.html

[Q06] 删除列
来源：http://hz.sufxvd.cn/gtyybeovpj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gtigfcblkw.html

[Q07] 删除表
来源：http://hz.meibo888.top/gtfxcacmmt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtmozwfymt.html

[Q08] 创建普通索引
来源：http://hz.cheryme.top/gtgkjmbkqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.andypj.xyz/gtmdknxqhu.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gttvytoyye.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtkkldtbut.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtvhvpvjjn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtckxkriws.html

[Q11] 一次插入多行
来源：http://hz.daxiang520.top/gtapkthyba.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtohtulpfh.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtiqbjeukf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.andypj.xyz/gtvhhfspav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtvdwcdbbi.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtjrpbebol.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtihvdilwq.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtaeasuamd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtujaqfhcq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhixingplan.top/gtbqzscvkw.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gtgrwznozu.html

SELECT * FROM users;
来源：http://hz.daxiang520.top/gtfttpzwyz.html

[Q16] 查询指定列
来源：http://hz.yonumen.top/gtnrnuptng.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtegikarjz.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtjslrskpx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhengqikj.top/gttzxxgfri.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gthkatdruf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgufenzy.top/gtzoosuwyn.html

[Q19] 范围查询
来源：http://hz.jinghuilouyu.cn/gtpovymmpk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtjwvlbhik.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtgvmcquey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gthdjlysez.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtlbfexxzs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtnvabumzx.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtppbydndn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtptrikykj.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtgajovmzr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hongshengwenyu.top/gtftbwtcza.html

[Q24] 去重
来源：http://hz.yj20258.top/gtcudnslrt.html

SELECT DISTINCT city FROM users;
来源：http://hz.smart0.xyz/gtfdfbjpyg.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtjmbwftqm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtezizbewu.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtmayzhqhn.html

SELECT COUNT(*) FROM users;
来源：http://hz.hammf.cn/gtjneojpzn.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gthypcaljw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtsohvbnbh.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gtuqdrakoa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gtequkhbeo.html

[Q29] 最大最小值
来源：http://hz.fzhhl.top/gtxcijismb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gtoxtbbfus.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtzgytpifj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtttjsomie.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtrtgsowvs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ydzc1.top/gtyldhxrkd.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gtbowfxsgy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtwniqbelp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gtocseezar.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtkajyoaxy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pycfn.com/gtqmugazps.html

[Q34] 每组取第一条
来源：http://hz.redwolf501.top/gtmbnigkyd.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtffiurgxw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.feifeiyinyue.top/gtskfphyok.html

) t WHERE rn = 1;
来源：http://hz.sweek.top/gtzovmjhfn.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtbmgsykus.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtsgtsmarn.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtovjvblze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtxsijrvpw.html

[Q37] 右连接
来源：http://hz.hywenlv.cn/gtsuslhcss.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gtgbuqwpaj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtmfvjjirz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gtgopqmyui.html

[Q39] 自连接（查上下级）
来源：http://hz.gogol.net.cn/gthazzkeym.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuxming.cn/gtwpgeqfha.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtuwvkxixu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtadokpdxu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtfwcywlgp.html

[Q41] 多表连接
来源：http://hz.ivvv.top/gtwemuumor.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgfzy.top/gtqhzmoiog.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gtkxrzkyjk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ywan-chungtsiang.top/gtpmxyvelx.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtoqqiipcq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtodmgmydr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtgslqxime.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gtkjpioolb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtqcvnlhqa.html

[Q44] IN 子查询
来源：http://hz.mhx1999.top/gtgtwxcfhk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtvryopemv.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigfzy.top/gthapgzypy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gttnvgvjnu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.quarkkingdee.top/gtsxmzgoiv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gttoweyriq.html

[Q47] 与平均值比较
来源：http://hz.nwbrower.top/gtufsqxcio.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.birdmap.top/gtrvpzxylb.html

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtkmbqonho.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtplgcfdpz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtmviwrcln.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtnlfnigfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtpncixgcz.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtdzwkljyi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtstkoaive.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtubuuyust.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtiqiagzuu.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtfeonpzta.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtgtmowjqt.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtsadkoxuk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sysykeji.top/gtlekcpjlt.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtbpjbmkpf.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gthctcrdsk.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtegultwyg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtckyqpbqn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtankqegol.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yongpay.top/gthpqyfgpv.html

[Q57] 行号
来源：http://hz.nanxuanxn.top/gtedcsiyfl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sufxvd.cn/gtzrvgksoa.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtkkztfysy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtrqxkxaej.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtdwvvazpm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258888.top/gteytbxmwm.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxinkj.top/gtjxeeswwu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtpbxhehki.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtsthmrvho.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtevcbxapv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtzgrzyvvc.html

[Q62] 分组占比
来源：http://hz.xuanzx.com/gtrretsxkw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtrymhvnqw.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtgrfilgtp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtvzkzrdaw.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtvzardjmq.html

COMMIT;
来源：http://hz.nanxinkj.top/gttcssguoy.html

[Q65] 回滚事务
来源：http://hz.shzxlz.cn/gtmyxjmdkd.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtkgnznggb.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtmxcrczys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuxming.cn/gtgwhaiidr.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gthqfcsbxr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtuskmmqme.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gthhkkhrgt.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtxorhbclk.html

ROLLBACK TO sp1;
来源：http://hz.chenzaomai.com/gtspphhlsb.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtaorisghw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtrceczgjy.html

[Q70] 更新统计信息
来源：http://hz.fengsongda.top/gtcexsjikq.html

ANALYZE TABLE users;
来源：http://hz.fzhhl.top/gtyjouwdci.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtpwwkaesj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtucdyvcoy.html

[Q72] 查看索引
来源：http://hz.yueranfly.top/gtfvflzmaf.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtrptzozak.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtilxdcpya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gtskeujjgj.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtdaqgnbuk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtkgvfusdf.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtcufuybby.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gttzrysoul.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtjpxptbxu.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtnbgpfkxm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gtbiosvblr.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtmbyzcrsr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtezrwquqo.html

[Q78] 当前时间
来源：http://hz.cdnleiting.top/gtnoewovfi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtpwexuthf.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtjuonprgv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.kuanghao11.cn/gtvbrfeqly.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtvbpmfpel.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxuanxn.top/gteijgcprc.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtppmfyfkt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ivvv.top/gttqrhopip.html

[Q82] 字符长度与字节长度
来源：http://hz.bjfxy.top/gtkvnnosfk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtxdcclqrl.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtdwircqzl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtolizzott.html

[Q84] 去除首尾空格
来源：http://hz.sufxvd.cn/gtxxxluoor.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gthbcpcaai.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtdcqsawrb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gtdccswkbe.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtisojegdz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gtavqnutxu.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtpectegyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtdtqdpufa.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtdppodrgk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.svipenyu.cn/gtpxyzmtjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtxxvihder.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtlpmfepjf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtavulnftc.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtwkxpxcbn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.feifeiyinyue.top/gtbzxffbcw.html

================================================================================
来源：http://hz.yonumen.top/gtsxmnhfqn.html

R. Bash 专题
来源：http://hz.yonumen.top/gtoxaziwfp.html

================================================================================
来源：http://hz.tianlin.xyz/gttwzjktyp.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gtxwqaxemj.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtlxauelrp.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtffbgnbow.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtsfnadtzn.html

name="Tom"; echo "$name"
来源：http://hz.andypj.xyz/gtjgstsddd.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtltfdbzcq.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtnrevvrqp.html

[R04] 位置参数
来源：http://hz.0kj1m.cn/gtrpiatfsq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gtdshhkxgi.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gttnjtucwh.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtqnuhexut.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gtoctgokqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtjucofjvs.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gttxdtouax.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtggskfkip.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtypsdcbgv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtinmwrqhf.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtikmhnajb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtycsekmqh.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtgiptdfzp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtwkwzxlxz.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtqruazyjq.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtqlrzjgum.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtodwvuizz.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtcdhyjhmf.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtpurnarqi.html

esac
来源：http://hz.nanxinkj.top/gthdhlspuq.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtreboqyfe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtsljmuqib.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtfjvzdbcz.html


<!-- 参考信息 -->