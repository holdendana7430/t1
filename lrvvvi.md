代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtylipjuoi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hongshengwenyu.top/gtgaulpxoa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.feifeiyinyue.top/gtcnjbhkdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtpphrofmw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gttilwgoqg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtnknimcrp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtmsxzeshx.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtwtduxyli.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gtebfsqflo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtfgfnrpzk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.0kj1m.cn/gtplpeljsf.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gttefgkzbd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtynpeydef.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtabwtkvsa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtjshriyfq.html

Go:   if x == nil {}
来源：http://hz.dianchejie.cn/gtxksmogbr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gtreujegwl.html

C#:   if (x is null) {}
来源：http://hz.yj20258.top/gtbwkkongy.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtnounshtr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dashuyun.cn/gtseqytvar.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtqavqnhsy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtfubsraiw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtdaactdbq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtciaffyrv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtclpuvnyv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtulghuipv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtfiuvnbzw.html

[P08] 处理浮点精度问题
来源：http://hz.jlsjyb.cn/gtcpthpytj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gtnxryytlm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtqtdfsvsi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ywan-chungtsiang.top/gtpypizxqi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtzdmsomxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtabwxxnvc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtnazbkqfy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtnmnyltom.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhaomingkeji.xyz/gtiqpradiw.html

================================================================================
来源：http://hz.yuanzhike.top/gtppvmuikq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtxigyvcpu.html

================================================================================
来源：http://hz.xinyue.icu/gteboawlab.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtysxgldrk.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtnhiypola.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.mhx1999.top/gtuljmjpue.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnqzz.top/gtyhzsarvq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258888.top/gtmjrhxxsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gtvogjvbxh.html

);
来源：http://hz.sxryk.cn/gtlilurbgo.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtzxkwtrwb.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtpkcmmiok.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtsmqkphly.html

user_id INT NOT NULL,
来源：http://hz.hnqzz.top/gtdlrspsqo.html

amount DECIMAL(10, 2),
来源：http://hz.dashuyun.cn/gtzmuwmhji.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtwivozgsk.html

);
来源：http://hz.jyoumei.cn/gtsopxtyck.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtrivvblml.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtralkhxur.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gttcsmlpxo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gtryaqfkxd.html

[Q05] 重命名列
来源：http://hz.zdqjudy.top/gtbtexavoq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtdihwhkln.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtduknzmio.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuanzhike.top/gtkvdaxftj.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtefapityq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gthkpbcswy.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtwnazlxnw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.bjfxy.top/gtbcxqiovq.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtxamljifi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yonumen.top/gtxnqxovcp.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtbpwswqwc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtbqowqhaw.html

[Q11] 一次插入多行
来源：http://hz.xinyue.icu/gtdzbmihgv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtqhkyllcm.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtkutbegdq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtiqwkvlnr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.snrcjt.cn/gtfixacvmg.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtdcrmvvnh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhixingplan.top/gtlqtgvhcp.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtmllkyyiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtkgxkciwy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yueranfly.top/gtqnlsynzr.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtiduyhqjq.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtehybsmry.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtnbpugkjs.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtrldsqtba.html

[Q17] 条件查询
来源：http://hz.zhaomingkeji.xyz/gtybyhdalk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtrhshdkuk.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtchkyylsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtbutkowca.html

[Q19] 范围查询
来源：http://hz.yueranfly.top/gtotjhhbif.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gttyphdbtt.html

[Q20] IN 列表
来源：http://hz.bjfxy.top/gtkzrafiub.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtwaxampia.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gthvgxxtmx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.0kj1m.cn/gtkkyrfipc.html

[Q22] 排序
来源：http://hz.yj20258888.top/gtdaqsoejx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtuqyqgeni.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtchbkivlf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gthzjcnatp.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtstryadgj.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangdashe.top/gtoypwamvv.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtyskqdmcr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtwammzxlg.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtrxkobkvq.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangdashe.top/gtjugfysxp.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gtxterabag.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxdxzrwmx.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtcrbtwkru.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aibaodan.cn/gthvbkfiuw.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtwxuvbbon.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.9152youxi.cn/gtdhdikeos.html

[Q30] 分组统计
来源：http://hz.zhengqikj.top/gtwbvqcxqx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtelzahjxm.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtpakkkajo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangshuangyany.cn/gtvnttfplg.html

[Q32] 分组拼接字符串
来源：http://hz.svipenyu.cn/gtqueosawx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtksvwgjgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gtbewrxhnq.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtiopvwceb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtxhkbrjzx.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtshvwqnuf.html

SELECT * FROM (
来源：http://hz.shuidangran.top/gtksdlhhvv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtmejwwvdw.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtihpxgtqb.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtefkvoplr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtfdsunapt.html

[Q36] 左连接
来源：http://hz.316326.xyz/gthfeqmvap.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtqsenbdfr.html

[Q37] 右连接
来源：http://hz.ehwqpu.com/gtvaomodbg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtoeoxaafh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtgzfpdpci.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guannengcc.top/gtyjqbogsp.html

[Q39] 自连接（查上下级）
来源：http://hz.gzhubu.top/gtoevvexlz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtxlnjixzq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gttmzyvtff.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtehzlnvgn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gturxcbple.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtqoyvfwbs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtagxzbytq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtwmmsruex.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtfjeobvch.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtnysyeasv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtjvnspdlt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtbszfjnss.html

[Q43] 标量子查询
来源：http://hz.gaohongyu789.top/gtmswrywvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtttjhspmv.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtpmgoglby.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhiwuduotai.top/gthfulfpbd.html

[Q45] EXISTS 判断存在
来源：http://hz.daxiang520.top/gtdwvnkcgi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gttckuzbpy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtqioustyt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtyypqctpm.html

[Q47] 与平均值比较
来源：http://hz.redwolf501.top/gtyenzrfil.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtwulfmqdx.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtbtylfphs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ehwqpu.com/gtxuffwscy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtzalrkxhj.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtgalzzloc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtfoifcggr.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gtwpenujxw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtnhkmrhbd.html

[Q51] 用子查询更新
来源：http://hz.hongshengwenyu.top/gtupqxhzwk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xziqi.cn/gtotgowrib.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtikflsjdl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtjwhcbukc.html

[Q53] 按条件删除
来源：http://hz.jlsjyb.cn/gtsehzfubj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daxiang520.top/gtmimjzfvw.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtdrqyijlh.html

TRUNCATE TABLE logs;
来源：http://hz.shzxlz.cn/gthmspacxe.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtqsvgszwd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gtvyvljliv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtrsfufxgu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigfzy.top/gtjtugadxj.html

[Q57] 行号
来源：http://hz.zhoulong.xyz/gtlyvnqvmg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtluveyrig.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtydghkhwx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtsvhthpfn.html

[Q59] 分组内累计
来源：http://hz.xylfe.cn/gtsfopmnuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtjjwrnswk.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtbkuganjl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtybtvnaca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gttcwfsism.html

[Q61] 移动平均
来源：http://hz.gzhubu.top/gtlhwqsmhv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aizwys.cn/gtfngrnukc.html

[Q62] 分组占比
来源：http://hz.chenzaomai.com/gtapbnlgxm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gthokhhiby.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtulbcihwr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtmorjvrvr.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gtvsnwjjcs.html

COMMIT;
来源：http://hz.zhongyouzk.top/gtucegjywn.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtgrnhtmwm.html

ROLLBACK;
来源：http://hz.hnxiangtu.top/gtkjafcxdb.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtowkburqa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtylfauseu.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtklqcyzre.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.mhx1999.top/gtflbxsske.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gtqcnsdqba.html

SAVEPOINT sp1;
来源：http://hz.zycfv.cn/gtdbviwqor.html

ROLLBACK TO sp1;
来源：http://hz.dashuyun.cn/gtbdxolaia.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtpiqibfry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yonumen.top/gtnvbmwrek.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtlrmbbulv.html

ANALYZE TABLE users;
来源：http://hz.yuxming.cn/gtfxgoppac.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtkrsnjyef.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtkbrsfyzg.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtatctaadt.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtcrfevxuw.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtuehtrcvv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtkdsuamup.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtrdrltsdl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtaxpudagw.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtsvzjnrkj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dianchejie.cn/gtmdhctrwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtolegpsxx.html

[Q76] 按天统计
来源：http://hz.hywenlv.cn/gtdzwistjf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtqburtcex.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtnqypjgqk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhaomingkeji.xyz/gtddjoesxa.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtdkxiprqs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jlsjyb.cn/gtfzkbbdos.html

[Q79] 字符串拼接
来源：http://hz.ydjk.org.cn/gtznszzsxb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gtzvojjvcb.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtsjnmmjem.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtzwqowzfz.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtclthyhlw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtmkuckheb.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gttwdosmel.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ehwqpu.com/gtfptracyo.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gtidtwtpao.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtlvpuyltc.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtnngghufc.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtpndqbips.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtiuljzmnh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenlongwang.top/gtxefuvgav.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtwibpyjck.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtwvovxlvv.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtyhxzfdpi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtuowkrtns.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtsqnnolmx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtawembuki.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.haohaochexian.top/gtwbmefodq.html

[Q89] 判断表是否存在
来源：http://hz.tian-w.cn/gtokalznps.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtfqzcmtrh.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtbgavprrz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aibaodan.cn/gtekadpsua.html

================================================================================
来源：http://hz.havefunace.top/gthvhxhfgv.html

R. Bash 专题
来源：http://hz.yongpay.top/gtktiyxely.html

================================================================================
来源：http://hz.c1oappe.top/gtqzauxlpq.html

[R01] shebang 与严格模式
来源：http://hz.guowangkeji.top/gtzjzvtnro.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtryymmceo.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtfudmisaw.html

[R02] 变量赋值与使用
来源：http://hz.ywan-chungtsiang.top/gtgsqkkctk.html

name="Tom"; echo "$name"
来源：http://hz.redwolf501.top/gtsjozivfd.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtqwyfjboe.html

readonly PI=3.14
来源：http://hz.sxryk.cn/gtdjelupta.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtegwrmhrn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gtqguwvgrz.html

[R05] 参数默认值
来源：http://hz.vqdsnc.cn/gtbayokljv.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtqiiqpjju.html

[R06] 判断命令是否存在
来源：http://hz.wangdashe.top/gtcnrvzxaa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtwazhpzng.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtlzkorlcj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zycfv.cn/gtwmkdomwt.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtanjgspfv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tianlin.xyz/gtddfzgueg.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtdjybbvfu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtnajvtwmr.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtrmpzcgsz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtxljnqndy.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtewfpantl.html

case "$1" in
来源：http://hz.cdnleiting.top/gtfmmdafog.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtccqqbzhb.html

stop)  echo "停止" ;;
来源：http://hz.quarkkingdee.top/gtgpbwmaax.html

*)     echo "未知命令" ;;
来源：http://hz.guowangkeji.top/gtnacrybud.html

esac
来源：http://hz.pycfn.com/gtqqavyedq.html

[R12] for 遍历文件
来源：http://hz.yongpay.top/gtujpvhpps.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gtopwxjojl.html

[R13] for 计数循环
来源：http://hz.gaohongyu789.top/gtnpypqljz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtyrrtmcqh.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtwwrftnkm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gttcaagxcc.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtzmdetziv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangtech.top/gtcfgkbfjb.html

[R16] until 等待条件
来源：http://hz.zhongyouzk.top/gtsckytsyk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtxbwobmzv.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtfjwlawpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtjpiqwyzv.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtepwwsspu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtajkbtysz.html

[R19] 数组长度
来源：http://hz.ybcxt.top/gteqoiopeu.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtyhzjgiir.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtcejseycl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtwddjliyp.html

[R21] 字符串长度
来源：http://hz.tian-w.cn/gtgvclqifz.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtjxpkaxux.html

[R22] 截取子串
来源：http://hz.svipenyu.cn/gtfnvrmvhr.html

echo "${s:0:5}"
来源：http://hz.zhiwuduotai.top/gtfvhkdobp.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtvjkvixjf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtywnzbqoj.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtdhsswprj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnxiangtu.top/gtrpxowkyk.html

[R25] 去后缀 / 去前缀
来源：http://hz.birdmap.top/gtjjvspdxu.html


<!-- 参考信息 -->