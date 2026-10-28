代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtmztowyay.html

C#:   if (x is null) {}
来源：http://hz.ehwqpu.com/gtsftocqfc.html

[P07] 防抖与节流
来源：http://hz.yuanzhike.top/gttzkrrnta.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gtdtnxdslj.html

PHP:  // 手写时间戳比较
来源：http://hz.xuetiantiany.cn/gtflkijqaf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gttxyaxgyy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtswjgazpo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xylfe.cn/gtuzrcynnu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtqjwzsjpx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gttxiwirbe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shangyingyoupin.top/gtsofyjoos.html

[P08] 处理浮点精度问题
来源：http://hz.jqgfzy.top/gtclajzyfe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gtxrjqybaq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gotoacloud.top/gtpcdkgfwg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtctdkdzon.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtmuxjpbbl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtajtjojob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnqzz.top/gtgivdmrlv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtphngfomo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydjk.org.cn/gtpwjifofr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtzalxrikj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gtgkikkpyu.html

================================================================================
来源：http://hz.hammf.cn/gtvclrwhed.html

[Q01] 创建表
来源：http://hz.cucudq.cn/gtblwfeuet.html

CREATE TABLE users (
来源：http://hz.tian-w.cn/gtokedmjea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtkmrkxpat.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtniffkdzo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtlktcxmee.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtelublmrn.html

);
来源：http://hz.gogol.net.cn/gtaweqdxhx.html

[Q02] 创建带外键的表
来源：http://hz.haohaochexian.top/gtiowevxpc.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtrnnjexqj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtjonvvgmi.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtyfwyevoq.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtexioxrsj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daxiang520.top/gtvyefbrop.html

);
来源：http://hz.birdmap.top/gthxevqxwc.html

[Q03] 增加列
来源：http://hz.yj20258.top/gtbkatsiur.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gthqcfnejd.html

[Q04] 修改列类型
来源：http://hz.xingfuxueyuan.xyz/gtvakdsurd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtjsmwhmkh.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtoicmtjpk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtrtcpwwif.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtocwudggx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtkrfoglvz.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtifqegljf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dashuyun.cn/gtumhcvzht.html

[Q08] 创建普通索引
来源：http://hz.gzhubu.top/gtmxixhcql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtdzzbuhpb.html

[Q09] 创建唯一索引
来源：http://hz.zhaomingkeji.xyz/gtnovxzwmy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtmrnsqlog.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtinlvwsbe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtenfowkmo.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gtznqlfawr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gtpoqacrwh.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtfigptwiv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gthflrrlos.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtfxgfhlin.html

[Q13] 忽略重复插入
来源：http://hz.wangshuangyany.cn/gtlleixjia.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenzaomai.com/gtnzlznvfw.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtejqnvtpi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.9152youxi.cn/gtyrqpcxkz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xinyue.icu/gtplkzyrsu.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gtjqelurzx.html

SELECT * FROM users;
来源：http://hz.vqdsnc.cn/gtbxniapic.html

[Q16] 查询指定列
来源：http://hz.jinqigfzy.top/gtyppbuiey.html

SELECT id, name FROM users;
来源：http://hz.hfpthk.cn/gtrxduwvzr.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtfxcuqtli.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtbwfvybed.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gthzylkvvx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtxwqcujpa.html

[Q19] 范围查询
来源：http://hz.cqqwz.cn/gtkzkyuaoe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.52xcode.cn/gtdibdurlx.html

[Q20] IN 列表
来源：http://hz.smart0.xyz/gtuopuhewp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtgiehwtri.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtvgacjvbq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtfleaqwyj.html

[Q22] 排序
来源：http://hz.jianghu66.top/gtgxazafve.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuanzhike.top/gtfunrngbb.html

[Q23] 分页
来源：http://hz.gaohongyu789.top/gttweagqwm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtjdepkqxo.html

[Q24] 去重
来源：http://hz.wangdashe.top/gtvinuihbi.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gtzsiuecld.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtryhvcjpj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtcixvrwve.html

[Q26] 计数
来源：http://hz.yongpay.top/gtyuidbsts.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtvzydatlf.html

[Q27] 条件计数
来源：http://hz.svipenyu.cn/gtgnxltear.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtubnqgost.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtlwaopvhp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtsftfiuvp.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtjmxrzwwi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cheryme.top/gtbkdxnmsz.html

[Q30] 分组统计
来源：http://hz.ehwqpu.com/gtedgfvocl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtuoenfprd.html

[Q31] 分组后过滤
来源：http://hz.cdnleiting.top/gttizgzrnq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtlvndavzw.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtygyxcgpo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtjsnzzipv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258.top/gtorlydlov.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtcsnukzfo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtdijxrrvq.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtgaelrvxw.html

SELECT * FROM (
来源：http://hz.shanyushiyangkeji.top/gtgaoogows.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yongpay.top/gtfnafusjy.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtmrqifydt.html

[Q35] 内连接
来源：http://hz.yonumen.top/gtvgngfrtf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gthgaciwof.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtqwmdxgpq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtsmosnoqk.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gthbfelnam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zycfv.cn/gtfkkmtrtw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jyoumei.cn/gtkoveisqi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtxftcuvrk.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtnbmgmbta.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gtlgslossn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.9152youxi.cn/gtjsuqfteu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtgkevffym.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtpnmvncmp.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtqtviacaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtotcjrwqj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenlongwang.top/gtgouncjnn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtszcnmqyp.html

[Q42] 连接条件附加过滤
来源：http://hz.zdqjudy.top/gtehphnzrh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.haohaochexian.top/gtewfnhmcp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuanzhike.top/gtatqdbjsk.html

[Q43] 标量子查询
来源：http://hz.aibaodan.cn/gtrvntkznb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtpwfmwmqr.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtrlhpikhc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenjidiqi.icu/gtwuqabpvc.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtcwzxpuwo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtjzjjiukf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtjeprcipk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtnbapzuvs.html

[Q47] 与平均值比较
来源：http://hz.snrcjt.cn/gtphfanfzw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtcinwykyj.html

[Q48] CTE 公用表表达式
来源：http://hz.yongpay.top/gtxvehimdz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gtkqfhkdoi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtulwgwoqm.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtoqjjizyj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtwytortsu.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtqcfuermi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gttrhtfvoi.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtjzwfemwj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtatdvqqwk.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtnkvpaywm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cucudq.cn/gtpuvbxqyp.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtxajcjkze.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pycfn.com/gthndjoydi.html

[Q54] 清空表
来源：http://hz.nanxuanxn.top/gtutuifebs.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangkeji.top/gtyvetvxqf.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtkgwmhyqu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtrhsqhtxx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daria6918.cn/gtuqlqehil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gthltqympa.html

[Q57] 行号
来源：http://hz.yvedp.cn/gtnrqzrcto.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gtwljtanvj.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtxsdbshwq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnqzz.top/gtqzdawuuk.html

[Q59] 分组内累计
来源：http://hz.ydjk.org.cn/gtqjsfulcw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtudugtavl.html

[Q60] 取上一行 / 下一行
来源：http://hz.iojbl.cn/gtxhnlfhdm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtnmcbeyid.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gttxkakonq.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtfnwambiy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtetywkhzz.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gttbnvgrsw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gteggyzxhr.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtbruorvlg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gthepngtbz.html

[Q64] 提交事务
来源：http://hz.zdqjudy.top/gtrfidwars.html

COMMIT;
来源：http://hz.jianghu66.top/gtmybqtkgt.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtueseduts.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtybynyjfy.html

[Q66] 行锁查询
来源：http://hz.daria6918.cn/gtekabnptq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydjk.org.cn/gtamttjimq.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtzwvsikun.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtqqsrczit.html

[Q68] 保存点
来源：http://hz.meibo888.top/gtsgdislix.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gttttosoxa.html

ROLLBACK TO sp1;
来源：http://hz.hywenlv.cn/gthhutpfvj.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtloohnghv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cqqwz.cn/gtvpvizlmq.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtavsukaql.html

ANALYZE TABLE users;
来源：http://hz.xziqi.cn/gtzxyyisry.html

[Q71] 查看建表语句
来源：http://hz.redwolf501.top/gtywqbphpr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gaohongyu789.top/gtcnieopvr.html

[Q72] 查看索引
来源：http://hz.cheryme.top/gtcwpvvkkm.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtmufpvcvc.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gtjmerpofm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtmyglkckz.html

[Q74] 强制使用索引
来源：http://hz.sxryk.cn/gtlekoloft.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtcptqtror.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtqrwyxhrv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gtucydunrf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ehwqpu.com/gtjnxaiovy.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtjcczntgm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtrwunytub.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gteefexynk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtultekiih.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtmfgpynlv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtdiqkjwfg.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtixmcixvr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtavlpzhvt.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtiuggcbmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtkrwexthx.html

[Q81] 字符串替换
来源：http://hz.dianchejie.cn/gtnjduxgpb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtpuevopyt.html

[Q82] 字符长度与字节长度
来源：http://hz.birdmap.top/gtxefrklch.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtjklhtvuz.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtpzqtajkl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtkazzcebd.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtlnmhxlhm.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtjbmokhdl.html

[Q85] 数值取整
来源：http://hz.smart0.xyz/gtmvltbkqr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gtitojlghx.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtxhvhqieu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.svipenyu.cn/gtaujfkcdv.html

[Q87] JSON 字段做条件
来源：http://hz.fzhhl.top/gttbapxagj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtfoxtiimp.html

[Q88] 行转列（条件聚合）
来源：http://hz.aizwys.cn/gtffajwydo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtfzohgtko.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtsnvwfbpa.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtfojuqgos.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtezklvwih.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtuixntzic.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtaecucemj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtafuejtrq.html

R. Bash 专题
来源：http://hz.yonumen.top/gthmoszewm.html

================================================================================
来源：http://hz.smart0.xyz/gtmseobffj.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtzvtnvpct.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gtlmrztosq.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtxikpbedh.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtuaijyfni.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtseysvglq.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtdziyznsa.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtlxynpoja.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtjvkzkrvf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtxqxdzdjr.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gtlbroaooy.html

name="${1:-default}"
来源：http://hz.guowangkeji.top/gtgzxehfms.html

[R06] 判断命令是否存在
来源：http://hz.vqdsnc.cn/gtvkieuxgh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtijikpqwt.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gteemzosyb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gttkassftd.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtojpgugcd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xinyue.icu/gtnfipvyvc.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtgxghmgbz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtzbhajpkr.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtlydhvyhs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtrlbiovpf.html

[R11] case 多分支
来源：http://hz.bjfxy.top/gtgqksetjr.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtsxpowczn.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangtech.top/gtchwlknie.html

stop)  echo "停止" ;;
来源：http://hz.jyoumei.cn/gtrbmcitsj.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtdvvxryme.html

esac
来源：http://hz.zycfv.cn/gtvqqvxoqu.html

[R12] for 遍历文件
来源：http://hz.yangfankeji.com/gtrtyhrdak.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aibaodan.cn/gteasfdalj.html

[R13] for 计数循环
来源：http://hz.pycfn.com/gttnnxdgvx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtfepnkoxl.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gtyrjrrfvr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgfzy.top/gtwxleiznx.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtvxgcnhuw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtwwqhwtmn.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtntjfcuwk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gteroxnapq.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtxmmcsiou.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtrslgnhml.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtgjosxbjr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtdajzyqax.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtnfyghqww.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gttynmxest.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtmrhjacqr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtvupsgfiy.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gtygsnrfyt.html

echo "${#s}"
来源：http://hz.shangyingyoupin.top/gtapwzcqdt.html

[R22] 截取子串
来源：http://hz.hammf.cn/gteewreisl.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtovtiwibq.html

[R23] 字符串替换
来源：http://hz.ehwqpu.com/gtjdyvffzf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gteelshgfn.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtuvzpuzfv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtwublbmkt.html

[R25] 去后缀 / 去前缀
来源：http://hz.havefunace.top/gtyvpqutsp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtoteogvml.html

[R26] 命令替换
来源：http://hz.cashguo.top/gtsibwlzll.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtrqluihev.html

[R27] 算术展开
来源：http://hz.aizwys.cn/gturcjyizm.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtavixoqpq.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gttuliaage.html

echo "scale=2; 10/3" | bc
来源：http://hz.jianghu66.top/gtiorsytkg.html

[R29] 定义函数
来源：http://hz.ybcxt.top/gtiwtdulwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.smart0.xyz/gtwdeftffu.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gtdcsvoxfs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dianchejie.cn/gtdhijztte.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtiqjccdvx.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtpgbpoppz.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtcsqoxboi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.quarkkingdee.top/gtiefqgxpv.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtvzpyiocr.html


<!-- 参考信息 -->