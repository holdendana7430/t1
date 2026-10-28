代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gttompqfed.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yueranfly.top/gtnvzfgzpk.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtcrusuyya.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtyaznbytv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtbmofxfsl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtjsegbeew.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtoeyibxdx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtsbypeszx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtttphseyx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtrhutfqor.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtkitihwht.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtegodcdli.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtsqifazuc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gtllabhmmj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gthvkintdm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtwkdgndep.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xziqi.cn/gtuzozcbuq.html

Go:   len(arr);  len(m)
来源：http://hz.chenjidiqi.icu/gtmxuqudmy.html

Ruby: x.length;  x.size
来源：http://hz.xingfuxueyuan.xyz/gtkgldbemg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtqkeuonet.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fengsongda.top/gtcccwdzkm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.9152youxi.cn/gtoiyvuffw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jlsjyb.cn/gtlfqrmmuv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtmjoupkqr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtmcnylspy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtigfwyrhg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtnryvnzkz.html

Ruby: a == b
来源：http://hz.316326.xyz/gtyumkyfew.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtkqcwrraw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shzxlz.cn/gtrbbdlcia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pengpengdd.cyou/gtukyswovc.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtnuazxphj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xinyue.icu/gtytglzgju.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtqvztacbu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtkxatdsaz.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtigpqolct.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtzpmohlkz.html

C#:   if (x is null) {}
来源：http://hz.yangfankeji.com/gteojzdxcy.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtjsrtbvfg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxuanxn.top/gtmarmaply.html

PHP:  // 手写时间戳比较
来源：http://hz.cheryme.top/gtssmfsvse.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtieruooyi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtucxvrkbv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtendfadeb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtycmsoerm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtuitcqwoq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtkjqexgbd.html

[P08] 处理浮点精度问题
来源：http://hz.ivvv.top/gtvigrwobn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fzhhl.top/gtufytecgh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aibaodan.cn/gtiwugavfr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gtyfbqltyc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydzc1.top/gtmbbjooyg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtmwonkrmg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.feifeiyinyue.top/gtpudtunlr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtjukaxrin.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.mhx1999.top/gtfgnstkpl.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcckpnmih.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gtnajzdtov.html

================================================================================
来源：http://hz.ybcxt.top/gtufuwfuvr.html

[Q01] 创建表
来源：http://hz.xuanzx.com/gtbsqywauj.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtthoyhdwg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtzpjhdckt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtokgkiyku.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtaqzeyxro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenzaomai.com/gtosvqhrhk.html

);
来源：http://hz.yueranfly.top/gtkhnrpnca.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtbbpfrjjx.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtlclgyxme.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtopmvtkqy.html

user_id INT NOT NULL,
来源：http://hz.cucudq.cn/gtpkzfsibx.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtsoviglnr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydjk.org.cn/gtkufibvpp.html

);
来源：http://hz.yongpay.top/gtaafcjaqx.html

[Q03] 增加列
来源：http://hz.dianchejie.cn/gtvwkvfgzv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gthxcgmrlr.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtdpaaopgd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtnezjykwv.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gtxobhabud.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtnsskhkge.html

[Q06] 删除列
来源：http://hz.haohaochexian.top/gtyxsundar.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtaetmkpzh.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtdcmwkfyh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.316326.xyz/gtljezsedt.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtdqxftpji.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtsizlmgzy.html

[Q09] 创建唯一索引
来源：http://hz.jqgufenzy.top/gtmlefqoop.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtpzkpjytq.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gtdyykqeeu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuetiantiany.cn/gtmlsciidp.html

[Q11] 一次插入多行
来源：http://hz.hywenlv.cn/gthmzzkbjm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtsjprqgbc.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtvzrzscik.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtuuqqimwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gtpnffrnlx.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtiuetzwwg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtzlrjanpb.html

[Q14] 存在则更新（upsert）
来源：http://hz.hongshengwenyu.top/gttdmpztpo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gthyxuagmi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hywenlv.cn/gtxgmiczee.html

[Q15] 查询全部
来源：http://hz.meibo888.top/gttvdsvrdm.html

SELECT * FROM users;
来源：http://hz.zhaomingkeji.xyz/gtumfkpreh.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtgciirpea.html

SELECT id, name FROM users;
来源：http://hz.nanxuanxn.top/gtbfmrldtl.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtdminhcdc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258.top/gtndckegti.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtftzqnvcl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aibaodan.cn/gtnpaanlkb.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtbfgrpthz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtvovivlkg.html

[Q20] IN 列表
来源：http://hz.aibaodan.cn/gtydtbqjqy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhijiandao.cn/gtczgakbsf.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gtlrngedzc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jyoumei.cn/gtsomqrqdz.html

[Q22] 排序
来源：http://hz.yj202588.top/gtwbxtrxqa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtlxszykdz.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtgnhtydfc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gtdecucvug.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtizpxnstj.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gthcquthzs.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtfadfcioe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtjbnvorxh.html

[Q26] 计数
来源：http://hz.yj20258.top/gtzouzaahc.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtiuczzfeu.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtxfegdkpm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fzhhl.top/gttkcrpjyd.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtonopktfa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtamqvpgly.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gtswmcdeds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtfqyasyja.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gtamduaevc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtvtokfedu.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtisltazts.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtmalvgyty.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtahqodyxp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtatptsnuz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gzhubu.top/gteqxbfpnx.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtjrbxvypl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtvjqlgcul.html

[Q34] 每组取第一条
来源：http://hz.hongshengwenyu.top/gtgyrcfglv.html

SELECT * FROM (
来源：http://hz.hysaishi.cn/gtwkboitfe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ybcxt.top/gteoifwibx.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtyhrdekcu.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gtfjsovwuj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtavusbogn.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtxvfkfera.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtyhnfjtcv.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtgewfsbhv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.smart0.xyz/gtueryqofi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgfzy.top/gtssmwxnko.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gaohongyu789.top/gtneapiosb.html

[Q39] 自连接（查上下级）
来源：http://hz.bjfxy.top/gtdepxhuqb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pycfn.com/gtiygqjqds.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gttlhkxkff.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtqschuusp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhixingplan.top/gtzunduswy.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtfamdpjwn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtgltwjqkk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtakwfuyhz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtmlmzsiov.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtlozgirjv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gttggjwvvl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cdnleiting.top/gtrcxazmck.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtuqitarjl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.snrcjt.cn/gtkoiskfgt.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gtztulgfrw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sxryk.cn/gtlqukpbxf.html

[Q45] EXISTS 判断存在
来源：http://hz.feifeiyinyue.top/gtiuajjsyo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtyptfrgpy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtznmghoxr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gttbligshl.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtaqcdehry.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gttmvpkouo.html

[Q48] CTE 公用表表达式
来源：http://hz.fengsongda.top/gtglvdqcti.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangdashe.top/gtfucrktzt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtwblwpgkm.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtlxhmejlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtpnzswcsm.html

[Q50] 批量更新
来源：http://hz.yj202588.top/gtauwptyxy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtorvsltcz.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtdavsuwki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gtnbycnppg.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gthtuhyyfv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtqyyvsumf.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtkehgavss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sysykeji.top/gtumyjzlyu.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtsztrnqxi.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtwarfvnop.html

[Q55] 排名（并列占位）
来源：http://hz.birdmap.top/gtzsdewtym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtvloekyec.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuanzhike.top/gtdzfmfnsh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtxvpfegig.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtmlwclpjn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenlongwang.top/gtilyxtxpk.html

[Q58] 累计求和
来源：http://hz.nanxuanxn.top/gthlykvrum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gthmbgqqyf.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtnzxidjzo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gttdubdsbo.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtwjslybcg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ehwqpu.com/gtvqgyuucp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daxiang520.top/gtutioaeco.html

[Q61] 移动平均
来源：http://hz.wangdashe.top/gtvrngjtre.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuetiantiany.cn/gtlddwdmbb.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtqlkkwvvp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtxspwlarx.html

[Q63] 开启事务
来源：http://hz.chenjidiqi.icu/gthhcyhrjo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtjauvqvaw.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtfzvaywrj.html

COMMIT;
来源：http://hz.jqgfzy.top/gttwziscyn.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtfubratuj.html

ROLLBACK;
来源：http://hz.52xcode.cn/gtlxdopzlj.html

[Q66] 行锁查询
来源：http://hz.zhijiandao.cn/gtrlbadexb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhongyouzk.top/gtncbeepwb.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gtytnjmmpn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtbzmwyzqk.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtndpytygj.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtqoyopnlj.html

ROLLBACK TO sp1;
来源：http://hz.zhoulong.xyz/gtprqukfih.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtoutxhlmh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinghuilouyu.cn/gthepgtmqc.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtzmgsjuav.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtcxmxdpbk.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtpaocqpqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtxswhbwxp.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtfqzbhujh.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtbhxegvnx.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtppaklhpw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtxmcbwkie.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtblzxofsc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tian-w.cn/gthdracdjc.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtraonwxpg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtacrhgrvt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gtnkblpfjf.html

[Q76] 按天统计
来源：http://hz.aizwys.cn/gtdjmlmfoe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtnhobapnx.html

[Q77] 时间加减
来源：http://hz.haohaochexian.top/gtuyjstfgu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtvzqaaevf.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtgkbucqsy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtvjfrthuy.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gttnhdxnyz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtgwzvaddm.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtoidpfrmu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtdpyjkqnw.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtmtruynzu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuxming.cn/gtreaptiay.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtytyzzgus.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gthavwkwiy.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtmesmygye.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gttyhavkgi.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtocgfnejc.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtegzgmrkn.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtnlwtukbs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtwqvqxrzg.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtygyrhbdv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtqogpteyo.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtbqzksiil.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtkpkaskwk.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtqqugvlgc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtkluvmfic.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtfzrxcjip.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtejvgoxfi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtpxmtwznv.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtdkqivfdu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jlsjyb.cn/gtjbhysbuq.html

================================================================================
来源：http://hz.snrcjt.cn/gtqeakztgh.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtlgndydlr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlorlrfgy.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gtizsnjtjt.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gthovccdye.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtjtbflqsz.html

[R02] 变量赋值与使用
来源：http://hz.hywenlv.cn/gtqnlniqat.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtrfisuwen.html

[R03] 只读变量
来源：http://hz.hnqzz.top/gtujszeaxt.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtqeidcrnl.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtnrokqzvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtscxwcevk.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtunpbskri.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtukcneqrd.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gtplyasdet.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtydbqzovk.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtlnhctsrp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtxofxjmux.html

[R08] 数值比较
来源：http://hz.yj20258888.top/gtbqqhbxok.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtbdlzkeql.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtjnysuwcn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtemmrcrzj.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtsxcxwsnn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtwppzrksy.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtcwhgably.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtmihsjlng.html

start) echo "启动" ;;
来源：http://hz.jianghu66.top/gtrklpelnq.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtciqinhdq.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtegodpstm.html

esac
来源：http://hz.kuanghao11.cn/gtmtfcbxqp.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gthfcfubrp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtaievhrzy.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtwtegnqfl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtnxzfwdow.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtclmndjdc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sweek.top/gtshmxfely.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtfnqzcyro.html


<!-- 参考信息 -->