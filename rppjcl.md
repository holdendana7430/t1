代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtwfuzxrnx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtxfrbloud.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtbvkscpkd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtyxufjxex.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtyeumufra.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtzfrihhcj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtxbimyoss.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtilmpdsaf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hfpthk.cn/gtxqaugzye.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gthtjgxsns.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.smart0.xyz/gtfsvoakdj.html

[P04] 求长度
来源：http://hz.zhaomingkeji.xyz/gtgdwdzrsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xylfe.cn/gtikwwxugq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtxxglvhqu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtfsiteswz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtensfonvg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtgujrqiso.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtsragatii.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtgmfargve.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtiovqaoqj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtwyajhcqg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtgtyrptur.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtnhpdqpjv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtevbvxhpg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtevqajbtc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.smart0.xyz/gtjaghggux.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtxmothvjg.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtaudjploo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gthlmkvkaw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtnoqbbgaa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtnobmevae.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gtbvfpufri.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtdikxjxqm.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtbxyvnjuf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtjpdbybds.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtirvnkjwe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtnzvjjaxp.html

C#:   if (x is null) {}
来源：http://hz.xuanzx.com/gtipiuvart.html

[P07] 防抖与节流
来源：http://hz.havefunace.top/gtsdyvuybr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gtxehnctiv.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtflsgddco.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtptzninoc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtvgtuluzv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtgvyiuvcf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtxwtrvzhl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtoxnhgfdy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtwdxaaulf.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gtqneimbra.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hfpthk.cn/gthdothmnr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenjidiqi.icu/gtpxhocikg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtipqzfgbh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtyvapolyw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigfzy.top/gtbzgejmss.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtcminqzpy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtfyzlsgmy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtvlrwalao.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzzsnaxhw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gthzinrxpq.html

================================================================================
来源：http://hz.ppjwa.cn/gthdltilsp.html

[Q01] 创建表
来源：http://hz.pycfn.com/gtugokcdlf.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtabblrbek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gttxcrudzs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtcbidyvlv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zycfv.cn/gteuopictz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtmgxixmzh.html

);
来源：http://hz.jianghu66.top/gtcqruhqgh.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtupvarzpo.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtfwydqxpw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtmlhcttas.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtoyzqlpon.html

amount DECIMAL(10, 2),
来源：http://hz.chenlongwang.top/gterwumirj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtnvyhlcdx.html

);
来源：http://hz.sufxvd.cn/gtlmudycpz.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtxjvjwbqb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtkvjpmkfo.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtlldgzzsy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gtvgxubglp.html

[Q05] 重命名列
来源：http://hz.shuidangran.top/gtkoaeylda.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtkyurlbzr.html

[Q06] 删除列
来源：http://hz.52xcode.cn/gtafiblxbq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sysykeji.top/gtwlzgfijm.html

[Q07] 删除表
来源：http://hz.meibo888.top/gtpzmvezql.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtfhbyxbru.html

[Q08] 创建普通索引
来源：http://hz.ppjwa.cn/gtdryqpwsp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cashguo.top/gtvsznctlo.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtldtzvxgr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtrzlusova.html

[Q10] 插入单行
来源：http://hz.zhongyouzk.top/gtkjkzegmu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cucudq.cn/gteaxwttlt.html

[Q11] 一次插入多行
来源：http://hz.hywenlv.cn/gtunnsklpb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtwyefyeqq.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtzxuyyhsl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jyoumei.cn/gtfhwhxywx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jyoumei.cn/gtdszblvui.html

[Q13] 忽略重复插入
来源：http://hz.jyoumei.cn/gtqvdkatji.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtekvoqsde.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtzlmoxvbr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtezhfcfgp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangshuangyany.cn/gtqdborfbq.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtapscplke.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtljqkhlrg.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtkisndtia.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtfipgnogr.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtvvrwkjlh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtcmkluftd.html

[Q18] 模糊匹配
来源：http://hz.smart0.xyz/gtuyezjvye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ehwqpu.com/gtrgptouiw.html

[Q19] 范围查询
来源：http://hz.birdmap.top/gtrmulmblk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtuntdyfpz.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gtznechcsq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtsilyezmx.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtqrowkytf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtrquxmomn.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtxwrhljkm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gtojcojddr.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtpujuhqdt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gthhsekikc.html

[Q24] 去重
来源：http://hz.yonumen.top/gtfvsgaapd.html

SELECT DISTINCT city FROM users;
来源：http://hz.jianghu66.top/gtrbafzmuy.html

[Q25] 只取前 N 条
来源：http://hz.jianghu66.top/gtgerzzeqr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fengsongda.top/gttvmgucxf.html

[Q26] 计数
来源：http://hz.cashguo.top/gtwnkygeye.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtmardreoo.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtnxkqyyuv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtjsotaqzm.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtbsvmzxum.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtjeznnyhc.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtairyjfvw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fengsongda.top/gtgqctqnht.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtvvzmxbnq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtlzygaeya.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtobkhlftg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtanupkzzm.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtmirldqbn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtcmeadapv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtkthqjevm.html

[Q33] 多列分组
来源：http://hz.zhijiandao.cn/gtjvagkizx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cucudq.cn/gtrkenjtcj.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtcirnavuf.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtueythqaq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gtgxbthmkr.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtdaklhxuk.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtlkufzjbg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtwgfbfoii.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtruutjfxd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gthedpmwjw.html

[Q37] 右连接
来源：http://hz.yj20258.top/gtwloaumpa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtlorxbllw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtlxvjuamz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtcahclyby.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtqluikvuj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuetiantiany.cn/gtfwpgdlfc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gtnmfwtyem.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtppfdcqto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xziqi.cn/gtnkxvuisg.html

[Q41] 多表连接
来源：http://hz.chenzaomai.com/gtzjufluih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guowangkeji.top/gtarzkzvqw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gttomlczjp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtthyggldi.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gttrersfoo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtxyxaxvbm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtmoudgbds.html

[Q43] 标量子查询
来源：http://hz.yuxming.cn/gtvjnjsdwx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hnqzz.top/gtuqvthfga.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gthayuhgfs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sufxvd.cn/gtmecvrmxk.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtbcgqaovd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtgzkbkymd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtjffmsmjj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtzzxslyad.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtmjpqwsql.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sysykeji.top/gtfxovgpca.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtngsydjnx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gthdwbbcck.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhongyouzk.top/gtfhoqvmli.html

[Q49] 更新单行
来源：http://hz.zycfv.cn/gtluonmify.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtiulghzuw.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtmvztujds.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtgcbbhssu.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtghqzqllc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.feifeiyinyue.top/gttxaqlbit.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gthkxtsecj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtbwgcwcgj.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtqvbhvyym.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shuidangran.top/gtaikafwir.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtxolrecnv.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gttcexcxnt.html

[Q55] 排名（并列占位）
来源：http://hz.tian-w.cn/gtkkvxlred.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtqbwowtfs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gtolozfnki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gthfrkkrgz.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtyowigoxw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtggdkyokf.html

[Q58] 累计求和
来源：http://hz.zhaomingkeji.xyz/gtncjujout.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtezpctzme.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gthszvlpbi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.snrcjt.cn/gtyzaagbiv.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtdjrrmzvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtofmmtyoo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.quarkkingdee.top/gtrvfqmofp.html

[Q61] 移动平均
来源：http://hz.yueranfly.top/gtquvrgemr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnqzz.top/gtuyoqetmh.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtmkcjzmql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtlqbfdsuw.html

[Q63] 开启事务
来源：http://hz.hnxiangtu.top/gtnnhwkbwx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtbzoamltn.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtpnekoutv.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gtahmxccbz.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtazdymbys.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtbzezrcnf.html

[Q66] 行锁查询
来源：http://hz.zhaomingkeji.xyz/gtszkbvrxq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yueranfly.top/gtoztwmapb.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gtiuafrgwo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gthyukqkxo.html

[Q68] 保存点
来源：http://hz.jlsjyb.cn/gtteaepwbk.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtncvljdxd.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtyhasjozp.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gttbtjbxmn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtwgjawaye.html

[Q70] 更新统计信息
来源：http://hz.daria6918.cn/gtwtycsdjj.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtxwfqgjws.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtavcrlfsu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtzkdypbbq.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtllxglsnt.html

SHOW INDEX FROM users;
来源：http://hz.xylfe.cn/gttzswwtfd.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtjqrwyfcj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtwhkbtfkn.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtxbwnmqrq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtznjpkgan.html

[Q75] 日期格式化
来源：http://hz.birdmap.top/gtvkncaqqr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtugttrvri.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtwmoumxvp.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtjiuwvrfz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtktxroxtd.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtyjuprtwa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtijpleqgy.html

[Q78] 当前时间
来源：http://hz.wangshuangyany.cn/gtckczmyto.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gttmpshwhw.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtdjzegujr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtgkorquly.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtkvbvqeko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bjfxy.top/gthxwzxncf.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtgdyteyuw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtkmlnukca.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtagiopmjw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gtteqopetj.html

[Q83] 大小写转换
来源：http://hz.ivvv.top/gtmosczkrt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ivvv.top/gtahzsicij.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtagguezsv.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtbaeblgap.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gtfchkhwmy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtnaybrhkg.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtttzemsbl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtnxfedepe.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtahpvjpwu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtomybanmo.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtdrdtekap.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtkmzagjnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtvzzdngdj.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtwgyukzpy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtfvefxcxt.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtzprnqlpg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtjphmievb.html

================================================================================
来源：http://hz.bjfxy.top/gtfnmmuamd.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtgyvtxdwg.html

================================================================================
来源：http://hz.jinqigufen.top/gtukfhaane.html

[R01] shebang 与严格模式
来源：http://hz.0kj1m.cn/gtwalfnxrk.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtyxudzehn.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtopluyfgn.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtyewilrfu.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtpbvgprga.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtujfzfxuz.html

readonly PI=3.14
来源：http://hz.aibaodan.cn/gtyqritsfy.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtklugbqsl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jyoumei.cn/gtcojntsct.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gthkmywsyh.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtwzszrljn.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtgisbqkdt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.redwolf501.top/gtvcdlrqcy.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtjcgfznzd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtrupqqupr.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtzdeudmhg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtvwclnsod.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtnuwegdox.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgfzy.top/gtmkylxdop.html

[R10] 正则匹配
来源：http://hz.nanxuanxn.top/gtrqyzjbwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenjidiqi.icu/gtuykwkcsr.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtoutvlmar.html

case "$1" in
来源：http://hz.sufxvd.cn/gtsnfiexmp.html

start) echo "启动" ;;
来源：http://hz.aizwys.cn/gtmlsqqjgn.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtmskveoox.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtkpsxepsj.html

esac
来源：http://hz.jqgufenzy.top/gtydwxpqtw.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gthgfqwwkj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gtbfxrmaun.html

[R13] for 计数循环
来源：http://hz.xziqi.cn/gtiisamlom.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtvgazgpdt.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtsxcvvwok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gthakffviv.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtdoksoqmw.html


<!-- 参考信息 -->