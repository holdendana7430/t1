代发 wailian999

);
来源：http://hz.yanxiufei.cn/gtbupnlmol.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtrojwfrrx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtvynhwrxt.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtutpldffz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxinkj.top/gtnasxvejm.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtufzqzddq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yongpay.top/gtcdawvlmv.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtyqmkgjez.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.feifeiyinyue.top/gtorwfilxm.html

[Q07] 删除表
来源：http://hz.jianghu66.top/gtylrabuip.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtihdyihsj.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtkqdyaqwr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtjcpkeqcm.html

[Q09] 创建唯一索引
来源：http://hz.xylfe.cn/gtvthtptjb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtdrsrjdbv.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtvhtchyig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gthlsjwene.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtvpgchmci.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtrpqlsveh.html

[Q12] 插入后取自增 ID
来源：http://hz.cqqwz.cn/gtsmhyjsvv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtdstshanp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuxming.cn/gtadpcrynu.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtdrdvkzge.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtvrffkpnu.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtduutuqlp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cucudq.cn/gtwlkkkbva.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gtbgioxaja.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtpuwftnem.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtznaqjbzl.html

[Q16] 查询指定列
来源：http://hz.chenzaomai.com/gtgzexsgwm.html

SELECT id, name FROM users;
来源：http://hz.yangfankeji.com/gtspoutspk.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtrmrqpbrg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gteykrzumk.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtzmrwddic.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gtzksnaihx.html

[Q19] 范围查询
来源：http://hz.shanyushiyangkeji.top/gtdgsjmbol.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtripoxmig.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtkkyesgnb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gtwzuckktf.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtavxfahnn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuanzx.com/gtkldavzzd.html

[Q22] 排序
来源：http://hz.cashguo.top/gtthnxzguf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.andypj.xyz/gtcbosggpj.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtswsdqlqt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtsfldpypm.html

[Q24] 去重
来源：http://hz.yonumen.top/gtehnbnjtv.html

SELECT DISTINCT city FROM users;
来源：http://hz.sufxvd.cn/gtwbucvqlu.html

[Q25] 只取前 N 条
来源：http://hz.cashguo.top/gtfztzeppc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shzxlz.cn/gthcsgzcrc.html

[Q26] 计数
来源：http://hz.xylfe.cn/gttoxhuhwt.html

SELECT COUNT(*) FROM users;
来源：http://hz.sweek.top/gtabwmofgb.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtlcaqqebb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shangyingyoupin.top/gtlmjgzpnw.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gtqdgeughq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cheryme.top/gtpormxyug.html

[Q29] 最大最小值
来源：http://hz.jinqigfzy.top/gtpmemrhms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtqchwygxu.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtrxwfqwrc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtiigntyjo.html

[Q31] 分组后过滤
来源：http://hz.daria6918.cn/gthnrmldkz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gthwiizclp.html

[Q32] 分组拼接字符串
来源：http://hz.jlsjyb.cn/gtdkjcnpoy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtyskrcrqf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fzhhl.top/gtcgwrtuxb.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtbemjzxij.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gtalizfulj.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gtriszdvrq.html

SELECT * FROM (
来源：http://hz.yangfankeji.com/gtfezxpcgy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shzxlz.cn/gtdihyjage.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtrkdugtuj.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtfxbqmvvf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gthqpnkiih.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtedapiycz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtfszlbfnf.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gtxkmdrews.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtgpyothbr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.havefunace.top/gtcsxbxuuv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gthtohtnpe.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtkpavhnlg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtkaixfehw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtymeobhjq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gthkvaarel.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtvdzzathy.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtaimtquro.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuanzx.com/gtqedufive.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hammf.cn/gtpdbfgtks.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtcuuoczfc.html

[Q42] 连接条件附加过滤
来源：http://hz.zhengqikj.top/gtypphhstr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ybcxt.top/gtoprvbdlu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtdqtrkyed.html

[Q43] 标量子查询
来源：http://hz.cqqwz.cn/gtlviocvvf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gthtnmcofd.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtipxsenlz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydjk.org.cn/gtdlnzhjtq.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtthlcnytr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtzvkkoxcr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtgqwchbqm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtrydtnsgz.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gterotbvfx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.feifeiyinyue.top/gtnmdtwhgb.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gttiwahphd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtlhrwhtqz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtrvdkdbdh.html

[Q49] 更新单行
来源：http://hz.sysykeji.top/gtpwwphjlx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtdbfqbrxa.html

[Q50] 批量更新
来源：http://hz.guannengcc.top/gtvnqkydbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtpwseeimg.html

[Q51] 用子查询更新
来源：http://hz.jinqigfzy.top/gtlhzejgym.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtsjrhpjzw.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gtzmlqbzqd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtmeldwsnp.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gttwhafabl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gthgbfhwiy.html

[Q54] 清空表
来源：http://hz.sufxvd.cn/gtyhgcsckl.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtnabrottn.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtpclxunas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenjidiqi.icu/gtmbrkocvd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtuxjxyfrm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtxikarnhx.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtprchjekj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jyoumei.cn/gtwnxsrfnm.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtbhngrrkw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daria6918.cn/gtadztapca.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtolvndcph.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtylylukgk.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gthyywwskh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xinyue.icu/gtzemeutne.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtwrgazhuh.html

[Q61] 移动平均
来源：http://hz.yj20258.top/gtciearxcv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtgtgivmmj.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gthwsseftl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtfgxrfcnf.html

[Q63] 开启事务
来源：http://hz.jlsjyb.cn/gtecdmczev.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.c1oappe.top/gtogpqmvau.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtxfiiqbwv.html

COMMIT;
来源：http://hz.jianghu66.top/gtvwglbrrx.html

[Q65] 回滚事务
来源：http://hz.shzxlz.cn/gtofpcyzxz.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtjqmfftaj.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtdevdfavu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gttmpreeac.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtobaohvnt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtkvwnjawd.html

[Q68] 保存点
来源：http://hz.ivvv.top/gtyoisqzwp.html

SAVEPOINT sp1;
来源：http://hz.iojbl.cn/gtiwekjnok.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gtffndtsjl.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtrrkivokk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtckqjqxyz.html

[Q70] 更新统计信息
来源：http://hz.zdqjudy.top/gtnztrjuis.html

ANALYZE TABLE users;
来源：http://hz.pengpengdd.cyou/gtutztlkpv.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtgrrfxgel.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gticivugcc.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtrwbqidww.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtbgwdloib.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtcluwniqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtpuurrcnt.html

[Q74] 强制使用索引
来源：http://hz.jiagoushi.top/gtxqehvbpy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gttiyrfqyk.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtutmrdbge.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtrxttadpm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtaufthete.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtdarrocuo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fengsongda.top/gtykxrljak.html

[Q77] 时间加减
来源：http://hz.daria6918.cn/gtzcillyul.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtbmxlsxjq.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtjqjlqqnz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtmipivvpq.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtfywqljmc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gtaksejlef.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtdfwwehoa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtpppbixkd.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtdayuucpd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtsaeshrwl.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gthetwyabt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.redwolf501.top/gtqouicefk.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtbbfmawbl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gthbrgvure.html

[Q84] 去除首尾空格
来源：http://hz.shangyingyoupin.top/gtxmqevghe.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gttdezjsqs.html

[Q85] 数值取整
来源：http://hz.dashuyun.cn/gtzpgivyzt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtsydodgjs.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtkmhgrqfh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtjwemieob.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtmiygnbpw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gtpwtbwmem.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gttnfhfvri.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gtvkvvlvua.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtjpohudhg.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtfbpqmflb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtdhftnigb.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtwwkdrwkn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtegxnisbn.html

================================================================================
来源：http://hz.yvedp.cn/gtfhschpma.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtzmlqowtu.html

================================================================================
来源：http://hz.havefunace.top/gtvuemcgld.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtpyckskge.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtyooqntev.html

set -euo pipefail
来源：http://hz.yvedp.cn/gttounueoc.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtlwdpohoa.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtomcwgqrj.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtqcpctjvg.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtshsbtzfo.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gtnghhglge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cucudq.cn/gtmojiqwud.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gthymbfwoy.html

name="${1:-default}"
来源：http://hz.fengsongda.top/gttmcjnwhf.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtdfkeezge.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtcvymidji.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtcoklgfkr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtsbuuzqrl.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gtrpbqpwoa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtkebibckw.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gthanplmkb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtsweedyat.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtwfnnpcfl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.birdmap.top/gtztvnhdkq.html

[R11] case 多分支
来源：http://hz.yuxming.cn/gtusmpkkpp.html

case "$1" in
来源：http://hz.yuanzhike.top/gtqsjstkym.html

start) echo "启动" ;;
来源：http://hz.pengpengdd.cyou/gtbupgfxgn.html

stop)  echo "停止" ;;
来源：http://hz.fzhhl.top/gtqpmcedyn.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gtsgnrezgl.html

esac
来源：http://hz.zycfv.cn/gtfcgwdheh.html

[R12] for 遍历文件
来源：http://hz.cdnleiting.top/gtnebzvxfd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtdyqhmfdd.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtmykwihzq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtcwwrkglu.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtxshyukih.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtahchvgah.html

[R15] while 逐行读文件
来源：http://hz.shuidangran.top/gtzvqapmmn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj202588.top/gtvtlqsxqq.html

[R16] until 等待条件
来源：http://hz.hysaishi.cn/gtpuywmflb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtfhlxqtth.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtjwcboktt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtdbdtmllx.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtgyugpkji.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtiodnzdvp.html

[R19] 数组长度
来源：http://hz.chenjidiqi.icu/gtupjqcxjy.html

echo "${#arr[@]}"
来源：http://hz.daria6918.cn/gtzhmqavxw.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtwoyizjuh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtqbbytwor.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtdfkukhtg.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtbetidvqd.html

[R22] 截取子串
来源：http://hz.mhx1999.top/gtzzuduilv.html

echo "${s:0:5}"
来源：http://hz.xylfe.cn/gtbxaqunqc.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtutkbghxs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtiesdmwet.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtjkpzipht.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtmilnlhsn.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnxiangtu.top/gtumkmibln.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtqzdvzsqa.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtolnzuelz.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtfesmaixc.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtentrpwdh.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtyhwueuby.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtryayrkrr.html

echo "scale=2; 10/3" | bc
来源：http://hz.smart0.xyz/gtozuvhaag.html

[R29] 定义函数
来源：http://hz.haohaochexian.top/gtxdenfgdg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtxsgbeyof.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gthhijeold.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtjuxovjbv.html

[R31] 局部变量
来源：http://hz.xingfuxueyuan.xyz/gtkqjnafyp.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtgldgoaeo.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtyzznqowz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tian-w.cn/gtlnlumtik.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtlesgvmzy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtmdsjilav.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtagaiukss.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtyvchuifz.html

[R35] 后台执行并等待
来源：http://hz.ydzc1.top/gtcxjjzybl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nwbrower.top/gtcrdkeqaz.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gtvcmrkadh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydzc1.top/gtapficdlo.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtxfuwhztz.html

files=$(ls -1)
来源：http://hz.jinghuilouyu.cn/gtnfgfuaem.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtfvmbdyon.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gtwuwqlkoj.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtejsrtnyd.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtofseoicq.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtlbwjlpmr.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtbvioxzkt.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtyadbmnjb.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtdmspsfya.html

[R42] 输入重定向
来源：http://hz.zhiwuduotai.top/gtjktpymgc.html

wc -l < a.txt
来源：http://hz.ybcxt.top/gtzsbhbwax.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtecnmjegs.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gttllirqyj.html

[R44] 按修改时间查找
来源：http://hz.pycfn.com/gtlzwecvbp.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtbexnbkjl.html

[R45] 批量删除
来源：http://hz.pycfn.com/gtncwrcsdm.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtdeemwjar.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtgnkwtzgb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtajlceqaa.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtdaufrund.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ivvv.top/gtryjjqykt.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtdcrlbupj.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuanzhike.top/gtrhcghfer.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gttxwzamok.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gthcsyyont.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtshhtakwy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cheryme.top/gtzktfirfl.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtfioopvcw.html


<!-- 参考信息 -->