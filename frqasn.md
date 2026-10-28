代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.snrcjt.cn/gtjkmfrjns.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtbdozinqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtuhlkgqso.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtwlritgux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuanzx.com/gtruhtgoty.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtntnsajez.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hywenlv.cn/gtkxcdjidw.html

[P04] 求长度
来源：http://hz.redwolf501.top/gtnvcudejz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yonumen.top/gtuahgojvr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtcyvsdyvi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtlsuwibow.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtgbrrmdqn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.c1oappe.top/gtolffsehm.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtsfexyuoa.html

Ruby: x.length;  x.size
来源：http://hz.xuetiantiany.cn/gtjdsumwqo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtsqbwxwxe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtmxbnuqcu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jlsjyb.cn/gtgnbeaann.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtlwuwfkxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtuinmamat.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gtvsnvxsuj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtsvzecbsa.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhijiandao.cn/gtvrfasduv.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtkohllego.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtrqlbxzlh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cashguo.top/gthriqbplv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtuyxvmmgg.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtrdgjyvyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.redwolf501.top/gtdmrabecx.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangtech.top/gtjuzkfajk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtgweioddy.html

Go:   if x == nil {}
来源：http://hz.aizwys.cn/gtnxfvxkvz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtozfebvjm.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtwdgbsbxt.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtngkylxcd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtctpdussi.html

PHP:  // 手写时间戳比较
来源：http://hz.jlsjyb.cn/gtvkukaaxf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtxhabchlb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtsqbdjyrv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtddfngrdy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gtwvttvilk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtspkbouut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuetiantiany.cn/gtrcixawit.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtezdcaaor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhengqikj.top/gtlinxbtlg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtkomgfopx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtfabyeric.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtxkikeunm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtrfxmmxeg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ybcxt.top/gtjvbzxgaq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fzhhl.top/gtrmdyjmbr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtsxqiaznm.html

================================================================================
来源：http://hz.nwbrower.top/gtjdjjzbzo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pycfn.com/gtqbtnqfrd.html

================================================================================
来源：http://hz.sysykeji.top/gtwnwwtsqo.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtwvvsbydj.html

CREATE TABLE users (
来源：http://hz.nanxinkj.top/gtiisbvndd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtclldgwqq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtuebwnnki.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shuidangran.top/gtdkmmzesm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtukmekwuh.html

);
来源：http://hz.gogol.net.cn/gtetoyeuzv.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtlphjjbcj.html

CREATE TABLE orders (
来源：http://hz.yj20258.top/gtsepqtmkn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtwgvinpdz.html

user_id INT NOT NULL,
来源：http://hz.andypj.xyz/gtpgzumpwv.html

amount DECIMAL(10, 2),
来源：http://hz.xingfuxueyuan.xyz/gtbyyrrcqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtwcctqclh.html

);
来源：http://hz.jinqigufen.top/gtpvkfxalu.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtaefgdhfy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hywenlv.cn/gtohgufquq.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtoqbthcvu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sxryk.cn/gtbbfaqswg.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtsawvabhx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daxiang520.top/gtpwxvldfr.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtqgmhdadc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hongshengwenyu.top/gtxwfrifst.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtnhdcflyl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtlgwgscuu.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtyecbnqkv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guannengcc.top/gtarpoqenp.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtszhxpusp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtmtwtqyjx.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtuvpmzojx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cqqwz.cn/gtikuflpsf.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtsdgojlke.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtzxbjiwhs.html

[Q12] 插入后取自增 ID
来源：http://hz.hongshengwenyu.top/gtwlxabjcv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtmivhkhlw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtozeagkvi.html

[Q13] 忽略重复插入
来源：http://hz.jinghuilouyu.cn/gtckwxtlnn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gtkizsmvhx.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtxymugpmh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ehwqpu.com/gtfduekcue.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtxxfvjzjn.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gtwgafnuld.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtcbicyism.html

[Q16] 查询指定列
来源：http://hz.wangdashe.top/gtoworqhhj.html

SELECT id, name FROM users;
来源：http://hz.yonumen.top/gtmobgdurs.html

[Q17] 条件查询
来源：http://hz.birdmap.top/gtaexxylaa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhoulong.xyz/gtcejjykrs.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtiqnqjrew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dianchejie.cn/gtqmosdjnb.html

[Q19] 范围查询
来源：http://hz.aibaodan.cn/gtxawibnwa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gttxzjcttz.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtgtarzgtz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gthznddhkm.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtudemiijq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gtcvthmxgh.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtowklugpv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtirlsnpvo.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtgwhwgqac.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gtppnrhsly.html

[Q24] 去重
来源：http://hz.guannengcc.top/gtabvwfhmx.html

SELECT DISTINCT city FROM users;
来源：http://hz.xylfe.cn/gttniwogyx.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtuhapayon.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtwezyygxa.html

[Q26] 计数
来源：http://hz.316326.xyz/gtrritobad.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gtrvlmvbvr.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gthditvqnz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gtnfhacaos.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtxqwzsazg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtrjdjjviy.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtxgqgiyih.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ybcxt.top/gtmivugqec.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtcabqbvfv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtrndkplac.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtxjaoynvi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtkacgvjfn.html

[Q32] 分组拼接字符串
来源：http://hz.hywenlv.cn/gtcymjytxw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtgfpfvixa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtudfqmlar.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gtsnpkzuaf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gtwvouxkwr.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtbltmhomh.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtneirqick.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtmilfmwsz.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtozomnxzl.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gthmbsmnmh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtmtovyqfv.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtyfuflvlr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtsurnxfjv.html

[Q37] 右连接
来源：http://hz.shzxlz.cn/gtnibqhidm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtawkemwfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtfnarkeus.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gthqldwgjj.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtndbtujqm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ybcxt.top/gtaohbjuib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gtlzfbszye.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtlbbwkdqe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtcrqaofhw.html

[Q41] 多表连接
来源：http://hz.ivvv.top/gtrzbsngqk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sufxvd.cn/gtymndugkn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cucudq.cn/gtuslhhnjp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258888.top/gtqrhgmlgx.html

[Q42] 连接条件附加过滤
来源：http://hz.gotoacloud.top/gtrtipcnvf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtcsspqzgf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtzdcxujig.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtwqbiizfj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtibpesiln.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtdbjjrkgj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtfnjzaaep.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtawsfvhmp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtrnnvewlk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuanzx.com/gttjjakdpz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtmkysegrw.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtvhegczue.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtkaaqtzbr.html

[Q48] CTE 公用表表达式
来源：http://hz.tian-w.cn/gtvtdeytkt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shangyingyoupin.top/gtrvochopv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gtjjgqzbnq.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtqnweaxuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hywenlv.cn/gtwsvspjzj.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtrfedltqu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtcxehngom.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangkeji.top/gtiaeqoteq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtlpebvquz.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gttoreqtwa.html

DELETE FROM users WHERE id = 10;
来源：http://hz.0kj1m.cn/gttcqyugao.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtxqnwowlm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dashuyun.cn/gtatrfbewp.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gthvxmfdpj.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtoedcnbqc.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtcalzsqmt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gtqlqkljsa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tian-w.cn/gtczolfvhk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtmmkiegaf.html

[Q57] 行号
来源：http://hz.yongpay.top/gtlovaciog.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtujaymkbx.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtfawcvnod.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258888.top/gtfihrfksp.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gtblowdasj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtijrfwxfu.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtkixvhjzj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtzchqugei.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gttoaaqoss.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtnedbyyae.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cdnleiting.top/gtiwgdkcod.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtwwqwmztk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtixaqlijb.html

[Q63] 开启事务
来源：http://hz.316326.xyz/gtklvuxfui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gogol.net.cn/gtsuwwbjyg.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtqprgxttt.html

COMMIT;
来源：http://hz.shuidangran.top/gtqtcpuzzn.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtxnujeyto.html

ROLLBACK;
来源：http://hz.yueranfly.top/gtpbqyacrz.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtzstxfoqa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtiqobzmrk.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gthzfwhros.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtesismkzo.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtchqfpbuf.html

SAVEPOINT sp1;
来源：http://hz.yueranfly.top/gtyrjerkby.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtrrgncbxk.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gttmkcjbde.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtowoqrpvj.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtppiskfsw.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtghwerdpq.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtunfgzikb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtdbongmvl.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtvqfliuqd.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gtjpjqmfnu.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtyhpirfhr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhiwuduotai.top/gtabcqixns.html

[Q74] 强制使用索引
来源：http://hz.chenlongwang.top/gtjxwscpgj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtdgudypqm.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtdgngvpey.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtstwsfhwj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuanzx.com/gtsbszbrsm.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gttqhnbgjz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhixingplan.top/gtvawylaau.html

[Q77] 时间加减
来源：http://hz.kuanghao11.cn/gtoypmkmsv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtvjkbtsud.html

[Q78] 当前时间
来源：http://hz.sxryk.cn/gthatprjzb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258.top/gtqndoepsg.html

[Q79] 字符串拼接
来源：http://hz.shzxlz.cn/gtiecqbtgg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtvuiarmdh.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtehrupylv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtkeikzvdb.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtwzjobrsy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtleagkogx.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtosmcmpsv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenzaomai.com/gtcnnldaiv.html

[Q83] 大小写转换
来源：http://hz.gotoacloud.top/gtzhinmkdi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtaqwwxqds.html

[Q84] 去除首尾空格
来源：http://hz.yuxming.cn/gtjuppbick.html

SELECT TRIM(name) FROM users;
来源：http://hz.jyoumei.cn/gttmszweal.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gtuxjgkxff.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtrkghkwhj.html

[Q86] 读取 JSON 字段
来源：http://hz.gzhubu.top/gthyubafwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtnmmemgti.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtivmseptl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtttmgwlxm.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtmisbjvtx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtatpffrmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuetiantiany.cn/gtthcaefjb.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtwuapszfv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtflizbwxe.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gtklqixphc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigufen.top/gtmzmnglrr.html

================================================================================
来源：http://hz.zhengqikj.top/gtprdbbvgw.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtukjggmkj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfmnzjfoe.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtqztysrnq.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtzmqhzlpl.html

set -euo pipefail
来源：http://hz.yangfankeji.com/gticlcbmht.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtegeqccju.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gtrmzxonuc.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gtdzyvynbx.html

readonly PI=3.14
来源：http://hz.aibaodan.cn/gtkabloccy.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtcaebnzud.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jianghu66.top/gtkuocseen.html

[R05] 参数默认值
来源：http://hz.hfpthk.cn/gtixurscja.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtkhrpvwuv.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtvderfphn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtczibgdql.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gthnavltsy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtsweoaevg.html

[R08] 数值比较
来源：http://hz.sysykeji.top/gtarocrnly.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtgjdjjvvf.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtzwxwhxvb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.birdmap.top/gtcjekpwxf.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtilrgotsg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gttdzyriyz.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtlalyryiw.html

case "$1" in
来源：http://hz.redwolf501.top/gtlptcaeoy.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtbdpxawdu.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtrpjhnyig.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtqzskdomq.html

esac
来源：http://hz.haohaochexian.top/gtuvfiqked.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtlrcllhws.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gtpcffldfd.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtnojueeua.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtgrjghuuw.html

[R14] C 风格 for
来源：http://hz.tianlin.xyz/gtifygocaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtftmsbeer.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtikuseuva.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gteltcggmh.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtjtfjfdio.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gttbwvgfdw.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtzzpwjlpv.html


<!-- 参考信息 -->