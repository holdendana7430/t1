代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jqgfzy.top/gtlxaqerpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtdveqcofv.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtxcexkxkb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yonumen.top/gtnnzpuhxh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtdbybcdtu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtekwooejs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtreznhlxd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtxnzrimaa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtpaxsoyrv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtktjjubom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gtwudgwcxo.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtrsjmgttt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hywenlv.cn/gtpvaemhpe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gthxgpsglo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtcxqutsau.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtpnzslhek.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtpyboazpl.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtsizxfabc.html

Ruby: x.length;  x.size
来源：http://hz.daria6918.cn/gturmuwwpa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtidakmnyz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258888.top/gtqlvpvypp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dashuyun.cn/gtkzrkwhod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtfqidpuch.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangshuangyany.cn/gtmvtsnudp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtcpzktvsh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.52xcode.cn/gtkpqqmohy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtbkqpnmts.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtfaygcxef.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258.top/gtgogrtmyj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aizwys.cn/gtislcyglp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtwgxbxlek.html

PHP:  if (empty($x)) {}
来源：http://hz.yueranfly.top/gtnuxgvlgo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hongshengwenyu.top/gtwqyxjprv.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gtvqbwirhr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gthzvppvlh.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtyrgmuudy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gttsfmcmpl.html

C#:   if (x is null) {}
来源：http://hz.ydzc1.top/gtjkionafb.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtdoykdvec.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gttkrukuqe.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtdwhzvfik.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gthlyehhtm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtfjmwwfde.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtjhcetlou.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtpfjnoomq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtuqmrtoxw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hfpthk.cn/gtllzsticx.html

[P08] 处理浮点精度问题
来源：http://hz.yueranfly.top/gtkwrjexrs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangkeji.top/gtxqerrpki.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtgsbjqdct.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtcshlsiug.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhengqikj.top/gtzvvymkur.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gtminfwfxy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.birdmap.top/gtbhvouxld.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtehtsrjbr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj202588.top/gtpfvlilsx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnwkmrqaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gtkzlbtddz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbsnzhxdh.html

[Q01] 创建表
来源：http://hz.feifeiyinyue.top/gtusqgkobf.html

CREATE TABLE users (
来源：http://hz.chenlongwang.top/gtulnxafpn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtekxzrttg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gzhubu.top/gttnfpnsao.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtrleshxpv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtzkuycmnf.html

);
来源：http://hz.ydzc1.top/gtcwakmwhk.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtcczjeotf.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gttwbpbppc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtprrktdgd.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtmstrcdvc.html

amount DECIMAL(10, 2),
来源：http://hz.jyoumei.cn/gtjnwmcgjl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shuidangran.top/gtyzovnfqy.html

);
来源：http://hz.0kj1m.cn/gtvyppzsus.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtkrjvfkcw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtiwttrmfa.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtiymujawc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtraptkeyo.html

[Q05] 重命名列
来源：http://hz.feifeiyinyue.top/gtisianhwn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtidfrahpg.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtctutbvhy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sysykeji.top/gteqzewxps.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gtpyfcqtxh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtzeuybtdm.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gtugydrplx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtnzkxeyvb.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gtwdtioqtx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtpohbwoun.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtucchlmcg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.svipenyu.cn/gtskcfxxvk.html

[Q11] 一次插入多行
来源：http://hz.tanke756.top/gtutldzrjx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gthnkcaipa.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtvagyxzav.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtrgncgyds.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.9152youxi.cn/gtwqufdwag.html

[Q13] 忽略重复插入
来源：http://hz.yanxiufei.cn/gthxkmvhun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gthtquvgaq.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhengqikj.top/gtnrnewigu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigfzy.top/gtsexkecef.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtvgnyzspx.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gtvxbveqmu.html

SELECT * FROM users;
来源：http://hz.cashguo.top/gtpxkptpfz.html

[Q16] 查询指定列
来源：http://hz.jlsjyb.cn/gtzwlctldz.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtvbrarvir.html

[Q17] 条件查询
来源：http://hz.feifeiyinyue.top/gtkwbapyxx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ehwqpu.com/gtpbjofcqp.html

[Q18] 模糊匹配
来源：http://hz.guannengcc.top/gtethjffod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gaohongyu789.top/gturuoipzz.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtpdtnqxod.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtdarumpzx.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtqhxiqzyd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtczkwulhs.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtbuzvvzgt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtvanqnwdt.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtifnpepkh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtfijzujmn.html

[Q23] 分页
来源：http://hz.nwbrower.top/gtvtyciurz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtmxrgwckh.html

[Q24] 去重
来源：http://hz.snrcjt.cn/gtrtplwyzo.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtztmoacey.html

[Q25] 只取前 N 条
来源：http://hz.gogol.net.cn/gttkgjtrfx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jianghu66.top/gtyepkxizg.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtwflaathv.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtpuvmihdy.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gthlombksn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cucudq.cn/gtvhuoopiz.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtaicbkaru.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtpkgfypef.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtkorpqymy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydjk.org.cn/gtpxbfglvl.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gtcozyargu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtbmirsxvc.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtsnanyqfu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.c1oappe.top/gtinylysfz.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtiezcoeup.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtcjkjlpaa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jyoumei.cn/gtpjegmxor.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gthhjahnzf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gtpnletyhx.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtiifowvne.html

SELECT * FROM (
来源：http://hz.zhongyouzk.top/gtggmgiokl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtxkbsjnyg.html

) t WHERE rn = 1;
来源：http://hz.gzhubu.top/gtuvrwlupv.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtneyrvffq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gttkjleliw.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtaknxqcpy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtktbpaltv.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtngvukwwl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.bjfxy.top/gtgesslnfa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shangyingyoupin.top/gtptjowqcd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtvknxdixr.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtojwoblit.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtlagfibvj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gtxrmizesb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtmydgpcxn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.redwolf501.top/gtcalmgeug.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtoxlkfpvm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yonumen.top/gtaaqgnwjh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtnhdermen.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yangfankeji.com/gturzdmotk.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtcszxhngc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sweek.top/gtceqprqoj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtwhbcvjks.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gtwhbvrark.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenlongwang.top/gtvobbdzpe.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtltpaecdx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.kuanghao11.cn/gtpptsoefl.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtqgdecrrp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtegywbwov.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shangyingyoupin.top/gtzaymredy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtmdatankr.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtgzgydusd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ybcxt.top/gtvvbodbtg.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtnmfydgcu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.9152youxi.cn/gtcbrdgbac.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtsixwsyko.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtsijuwtfg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtqdjceaah.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtczmazwri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tianlin.xyz/gtrgkladak.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtbzquhvih.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtgwpkgjtm.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtpshjojux.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guowangkeji.top/gtkzpccslh.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtgbsgijmg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtelojlhzt.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtspwbtxtr.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gttuvukuvg.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gtxihhdinm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gtezklewij.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ppjwa.cn/gtjfkcnnul.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinghuilouyu.cn/gthrokvvfo.html

[Q57] 行号
来源：http://hz.haohaochexian.top/gtzhhobsly.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtdpliwqbm.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtlesvsoha.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtbozflqpa.html

[Q59] 分组内累计
来源：http://hz.xinyue.icu/gtowuwkxea.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtqevtcywh.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtdvybfkxr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtpicxuovd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gtywkmwgjp.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtyapywlzz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtcawymblo.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtlujwkssa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gthwywzcny.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtvfwzhdmo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nwbrower.top/gtigngglmc.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtbzbpgfnb.html

COMMIT;
来源：http://hz.daxiang520.top/gtezywkukx.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtycxrzelq.html

ROLLBACK;
来源：http://hz.jinghuilouyu.cn/gtgrmcfoky.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtxbgviozw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtvknbyszm.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtmnvduoxt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gteekiglpe.html

[Q68] 保存点
来源：http://hz.chenlongwang.top/gtxjsipdbq.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtztagfgyo.html

ROLLBACK TO sp1;
来源：http://hz.xylfe.cn/gtcmkxdfws.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtvprauuoh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtogziojjy.html

[Q70] 更新统计信息
来源：http://hz.yj202588.top/gtunzvooks.html

ANALYZE TABLE users;
来源：http://hz.zhijiandao.cn/gtevwxpkti.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtpmsoekou.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtlmsvfvam.html

[Q72] 查看索引
来源：http://hz.yj202588.top/gtsljbzncs.html

SHOW INDEX FROM users;
来源：http://hz.xziqi.cn/gtisvwhlgj.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtwewcbvkg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtqhmendyx.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtqlatxswx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhiwuduotai.top/gtqumzocdn.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gtostilxls.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtajkbrbyo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtrdmsomjy.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gterctbukg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtcnolnlnj.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gttswlzriz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtcsvimamf.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtvtqwwlzl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.smart0.xyz/gtsbvvoqnn.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtmsrlcrhr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtvuogqkos.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtunytotmc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtltdsdpsv.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtuingomvc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtsogvtasj.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtauiaqjvo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.meibo888.top/gtkgsmtmnr.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtzmvdbfun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtqjpjuwek.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtzioulyyv.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gtcnligdfn.html

[Q85] 数值取整
来源：http://hz.316326.xyz/gtlbnwjeya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtshktozjj.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtwejrxbdu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtygnrjkex.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gtvqhzxxml.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.52xcode.cn/gttdeitynd.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuanzhike.top/gtkcrdrnzy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fzhhl.top/gtbmdwbmii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhengqikj.top/gtbltzmztw.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gthjopkyif.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtshuaumli.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtlpcrdsku.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtvihpegpr.html

================================================================================
来源：http://hz.yj20258.top/gtdpzkmxmc.html

R. Bash 专题
来源：http://hz.0kj1m.cn/gtfqindnpz.html

================================================================================
来源：http://hz.xinyue.icu/gtqoedizwx.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtlnwiypyh.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtkliqnubz.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtddgwhior.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtppiwwzuc.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtzljietzm.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtzrxcpcvb.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtcxbrxaey.html

[R04] 位置参数
来源：http://hz.shanyushiyangkeji.top/gtiztvdbyj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtmgrslvvy.html

[R05] 参数默认值
来源：http://hz.0kj1m.cn/gtkrryoatz.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtjnalsafz.html

[R06] 判断命令是否存在
来源：http://hz.nwbrower.top/gtahkyuqbo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtvvxqpjrl.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtvyrfzppz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gogol.net.cn/gtyfuiykcf.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gthjadqege.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gtohqjplpe.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtozjpnuug.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtctqcghxy.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gtqqlzadns.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.feifeiyinyue.top/gtjlleewca.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtilayogdu.html

case "$1" in
来源：http://hz.jqgfzy.top/gtozqhyxea.html

start) echo "启动" ;;
来源：http://hz.shangyingyoupin.top/gtefetjcqf.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtzsrmkrkd.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gtzidprksx.html

esac
来源：http://hz.hysaishi.cn/gtlotlolqv.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtwozusylo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtjseynqex.html

[R13] for 计数循环
来源：http://hz.cdnleiting.top/gtdhtjhfiw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yonumen.top/gtlfjgnjxn.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtwqftfblu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtdamdojte.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtodkwehfq.html


<!-- 参考信息 -->