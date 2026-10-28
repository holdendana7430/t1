代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuanzx.com/gtpseormbz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtijuhazjd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtlvodiyie.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gtravqnuvc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jiagoushi.top/gtvknmvgrh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtyxciexdf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtsnwbuzhv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtbbhfapvy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtzxvbsglk.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtewpztkgp.html

Ruby: x.length;  x.size
来源：http://hz.zhaomingkeji.xyz/gtgrjohzwq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtdmwjxbzf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtrkcnnhya.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtmlshslvn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtofwcfhhl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtdznmotms.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtdojhmixc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guannengcc.top/gtguoongxe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gotoacloud.top/gtffpcruef.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtxqpzbihh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtxgwvvuqn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tanke756.top/gtxsndkvqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zdqjudy.top/gtongswdtz.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtrgztbqtg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtqgdaafrw.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtdsiwweri.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yvedp.cn/gtcgvejjda.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtveetaaqz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtuyxkhedi.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtyisngbdr.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtodrrelqm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj202588.top/gtbhksrjhm.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtpbbvginj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtvonkqrbg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtniuslicd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtlegspwkb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtqddquowl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fengsongda.top/gtecsvojhd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gttymziwad.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtkezdggdz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtdljuplnv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgufenzy.top/gtmqntsnpw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtcadgsuze.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zycfv.cn/gtvpgaxtab.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtbbjcekmj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtfprtlzfa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtelpwwvbg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtkhgibbxr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrqjpkqjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtxognquhj.html

================================================================================
来源：http://hz.jqgufenzy.top/gttcwfccku.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtxaysazye.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gttfqgwjal.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtjemxuobx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gotoacloud.top/gtrgujiynt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gtkqaozshm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtdyjtqkmd.html

);
来源：http://hz.chenzaomai.com/gtefkmhnub.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtfvnzpefu.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtjllcgkbr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtuqsohlyx.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtjeopqqmw.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtwrwpyzea.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258.top/gtoturzzgk.html

);
来源：http://hz.guannengcc.top/gtrhthwfww.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gtcfefwvka.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtxzrndwsk.html

[Q04] 修改列类型
来源：http://hz.chenlongwang.top/gtcppnsvvl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gtddjlclot.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtdsyhwodx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtgolfttwb.html

[Q06] 删除列
来源：http://hz.cqqwz.cn/gtfutvgmmy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.snrcjt.cn/gtunpvjqub.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtaufnbmhy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtkaumwesy.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gtbqduxowc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gttiomxskl.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtwekxgtqf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtubkcoxjz.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gtdqorknmi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shangyingyoupin.top/gtdtppmsma.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gtnnstwsfm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtxrrhvzmw.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtlehppdfy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tianlin.xyz/gtmweepqxr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtzojdmqvx.html

[Q13] 忽略重复插入
来源：http://hz.yuanzhike.top/gthpgzvnuz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtuxgcurma.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gtanvibqzr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tian-w.cn/gtlhtdspnr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtjiciwxrk.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtomxafphm.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtbiwrprzf.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtyzpaokrq.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtadkbrrat.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gttxwlgpfh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhengqikj.top/gtemjphvrt.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtsvmqntkx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtzsuqdisl.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtdjyqcmaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gtbbjaqvjt.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtjqczovpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.quarkkingdee.top/gtoijnpvyv.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtnengejaa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sufxvd.cn/gtowezrglv.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtbrypmbtx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtsuagkozx.html

[Q23] 分页
来源：http://hz.guannengcc.top/gtqbrnzprs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gtlmcwgmpl.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtgdgsbcce.html

SELECT DISTINCT city FROM users;
来源：http://hz.cucudq.cn/gtkfzsjvss.html

[Q25] 只取前 N 条
来源：http://hz.gogol.net.cn/gtxhwdohpx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gtagzmvlop.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtzhepeqoy.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnxiangtu.top/gtigfursau.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gthutrugkv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtcnocrrbi.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtpwrfxymn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtwrsknbnm.html

[Q29] 最大最小值
来源：http://hz.cashguo.top/gtqngjopew.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenzaomai.com/gtflygyizb.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtuzrsfwuk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtiylajlyz.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtagfeyrkb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hywenlv.cn/gtfvzysjma.html

[Q32] 分组拼接字符串
来源：http://hz.jqgufenzy.top/gtayzrjlby.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtiaqclzgb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtfsoeieui.html

[Q33] 多列分组
来源：http://hz.cucudq.cn/gthdniwwuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gteasggsfi.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtxnakameq.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gtvexikdbf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtyiqapynk.html

) t WHERE rn = 1;
来源：http://hz.cdnleiting.top/gtmimzgcdx.html

[Q35] 内连接
来源：http://hz.zhaomingkeji.xyz/gtjiwrkqyi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtgkaekqqm.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gtehalpxos.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gtfddtyfqr.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtlnpssyiq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtuojsbann.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shangyingyoupin.top/gtxdycqpzu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gthubnqhyv.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gttkofawlg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenjidiqi.icu/gtgmtxrjqj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtthskkkno.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtwprqfcxi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtqugfgmkq.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gtjhzkbsnw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtrgirbmwx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtzxbchxkq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtslylxfxm.html

[Q42] 连接条件附加过滤
来源：http://hz.cashguo.top/gtcvcdjbwk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtihcawsxx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sysykeji.top/gthpiyxcdt.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtjwjhqhsv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhixingplan.top/gtzbdwglrt.html

[Q44] IN 子查询
来源：http://hz.andypj.xyz/gtxybexilx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gtpfjcuvun.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gthuggotoy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtvvpyydwx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtqqkkigzy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtlvqjjdvb.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtotozbxdu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtkbfhjxwf.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtsgfexcue.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtfxjnvaef.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gtgahurtbj.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtigxetktr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtmdxglxjb.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtalveuxvq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtoqhhdrjh.html

[Q51] 用子查询更新
来源：http://hz.ppjwa.cn/gtcpragpkc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtzavvgrkg.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gtxilleynt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtqatnovzx.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtudjupzuy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtxwucxtyr.html

[Q54] 清空表
来源：http://hz.redwolf501.top/gtacqhpbuc.html

TRUNCATE TABLE logs;
来源：http://hz.pycfn.com/gtmokoaoer.html

[Q55] 排名（并列占位）
来源：http://hz.wangdashe.top/gttsvljisz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.316326.xyz/gtblhkoboa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yangfankeji.com/gtzcscszmk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtdcyiwofl.html

[Q57] 行号
来源：http://hz.yuanzhike.top/gtlcazegbx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fengsongda.top/gtvoyrwlzq.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtsnovtxoz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtksjzamqz.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtyeiaqbym.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhijiandao.cn/gtlwgbgmwt.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtiotwrkpv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangtech.top/gtnihycirp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtbzuaepjq.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtxqhkhaue.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guowangkeji.top/gtvqivpfab.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtzrtdijzj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtkldqlczu.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtfnzkqyxg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtvbubwzwr.html

[Q64] 提交事务
来源：http://hz.jinqigufen.top/gtwzqqioix.html

COMMIT;
来源：http://hz.fzhhl.top/gthhohnhzk.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtiunkxquj.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtdrmstsop.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtrjifspcv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtryoihvpk.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gthoabcehj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daxiang520.top/gteuzbdslf.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtiqiczjtv.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtbdohxjof.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtioakfwfi.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtrcwoatff.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jyoumei.cn/gtbjwbfzab.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gtdtyiuzyj.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtwszayfyk.html

[Q71] 查看建表语句
来源：http://hz.zdqjudy.top/gthfswxeyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtexlpeyjq.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtvqnehfby.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gtxkbiinsk.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gtrapzpira.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtrtcbvoxy.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtwwxyzwjw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gtwcyugvck.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtuwjrmldh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.mhx1999.top/gtdwqiawxd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.snrcjt.cn/gtqncykwag.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtygocjmap.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtrmzmrxcy.html

[Q77] 时间加减
来源：http://hz.xingfuxueyuan.xyz/gtjkukcqbw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtawjbrlfs.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtwxraahte.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtiqvnuoly.html

[Q79] 字符串拼接
来源：http://hz.sufxvd.cn/gttrbyhwfj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtnpbdjsup.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtmqnxxyic.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtfhuhcydv.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtsjgzyjlc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtnejyjxdi.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtaiiajlih.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtobmlytou.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtsbbwanlj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtqgxbqaxa.html

[Q84] 去除首尾空格
来源：http://hz.zdqjudy.top/gthftpeixt.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gttjixcgaq.html

[Q85] 数值取整
来源：http://hz.cheryme.top/gtjqthsaiy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuxming.cn/gtzycubpwt.html

[Q86] 读取 JSON 字段
来源：http://hz.havefunace.top/gtsvfknoix.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtkrauzhlb.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gttazvdroo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gtzzfhkxpx.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtmmancsac.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtbwojrmfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtdudpaick.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gttpqniwer.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtieaynkag.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtcfvzezas.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtatsvryad.html

================================================================================
来源：http://hz.daria6918.cn/gtxqyntxfy.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gtsjnuixgb.html

================================================================================
来源：http://hz.xinyue.icu/gtdxieodsa.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtdntvzozh.html

#!/usr/bin/env bash
来源：http://hz.cdnleiting.top/gtfkjtpren.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtlroutxlo.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtywwielvz.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtcrpnigrk.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtjwialuws.html

readonly PI=3.14
来源：http://hz.hnqzz.top/gttvbdcupr.html

[R04] 位置参数
来源：http://hz.chenjidiqi.icu/gtdsqbrogm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtvsqlspcb.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtkfmcztzk.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtyuoticrs.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtlthhecua.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtthcerfxx.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtsqskukug.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gtvouxwgrm.html

[R08] 数值比较
来源：http://hz.yuxming.cn/gtbbxgnizq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtggneceiz.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtljextorp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gtspvjjeum.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gterpgizrl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtymusnhbe.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtxuenmlii.html

case "$1" in
来源：http://hz.zhixingplan.top/gtejxyrwoi.html

start) echo "启动" ;;
来源：http://hz.jyoumei.cn/gtmiqfqxpy.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtiyiuepky.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gtfnctyrlc.html

esac
来源：http://hz.316326.xyz/gtaupsxalr.html

[R12] for 遍历文件
来源：http://hz.vqdsnc.cn/gtgvdoqeft.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtlkvllfvl.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtyhikpvgj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtjxpflios.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtwxwtfpwi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtstwmjfba.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtwdaogeya.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtepxfowfm.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtrqfxritv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtgqawjntn.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtmlxuicmq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtgjpnbpzw.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtdvtqufyj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gtndhnauwp.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtpidszdvh.html


<!-- 参考信息 -->