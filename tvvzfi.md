代发 wailian999

);
来源：http://hz.guannengcc.top/gtzynfpkpe.html

[Q03] 增加列
来源：http://hz.jianghu66.top/gtxjxmuffg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gtsjguuugg.html

[Q04] 修改列类型
来源：http://hz.52xcode.cn/gtuaqcefol.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtxertlvov.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtgxzucgzv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gthzrizbec.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtakrshuay.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtsvjabbab.html

[Q07] 删除表
来源：http://hz.birdmap.top/gtnkvwuhjl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gtfzpgfnap.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtdxhsplhy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guannengcc.top/gtogyxkwni.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtupxijver.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtddtfrhbe.html

[Q10] 插入单行
来源：http://hz.hongshengwenyu.top/gtkblhlzwl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtgycydyvh.html

[Q11] 一次插入多行
来源：http://hz.yj20258888.top/gtgwhaiiiu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ehwqpu.com/gtfopjopxn.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtcxnmwost.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtiqroltyu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gtxgcgfrqu.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtshnnqcgu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtpgdbwuwp.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtvowqehtu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtiwohsxqc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.quarkkingdee.top/gtbzdhavzu.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtxoxsrtej.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gtkzhzwyqy.html

[Q16] 查询指定列
来源：http://hz.haohaochexian.top/gtzevchmnr.html

SELECT id, name FROM users;
来源：http://hz.gotoacloud.top/gtgzcfbekz.html

[Q17] 条件查询
来源：http://hz.sysykeji.top/gtafuxyddx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gtflthyqvi.html

[Q18] 模糊匹配
来源：http://hz.zhiwuduotai.top/gtmtaxsyxd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtgmnbathp.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtjvicxzzr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hammf.cn/gtypqrszps.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtizmipnxk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtxqjmdmua.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtbadvayfe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtoqftrdjg.html

[Q22] 排序
来源：http://hz.shangyingyoupin.top/gtupzdclaw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtykkjgvgm.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtfyeqonag.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gtldqhbqyk.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtyoeijclw.html

SELECT DISTINCT city FROM users;
来源：http://hz.hywenlv.cn/gtshijydov.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtskjginic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtkbqlzmoo.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtjelmwktd.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtgekltevw.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtidwdwkwi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gtlzjnkljl.html

[Q28] 求和与平均
来源：http://hz.wangshuangyany.cn/gtrnokuubz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gtjajbwtzg.html

[Q29] 最大最小值
来源：http://hz.sweek.top/gtnkkbhdbj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtunwoyjyd.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtrljhnkcq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtjetylyej.html

[Q31] 分组后过滤
来源：http://hz.yvedp.cn/gtzszxyqhp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gtzrjavjdh.html

[Q32] 分组拼接字符串
来源：http://hz.hongshengwenyu.top/gtndfjyayj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtoozazjbf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigfzy.top/gtzwraptvw.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtordtvivq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gthhubyesf.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gtgkexphgr.html

SELECT * FROM (
来源：http://hz.ywan-chungtsiang.top/gthpuacfbl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtunrqtwsj.html

) t WHERE rn = 1;
来源：http://hz.jinqigufen.top/gtifpmcctx.html

[Q35] 内连接
来源：http://hz.yj202588.top/gttywlqokv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtzonbiyxt.html

[Q36] 左连接
来源：http://hz.yongpay.top/gtnauygcyo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gttqytuptt.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtawucxbup.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258.top/gtqlhynlql.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtpcqavfdi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pycfn.com/gtwjvqrjlu.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtrebuodvj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtzbrjbzlb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtcqearntf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtcjcmjcjm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gthcbwlhbk.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtzqwomvch.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtadpovyru.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtknmtwxta.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtfkepoxyh.html

[Q42] 连接条件附加过滤
来源：http://hz.sweek.top/gtkqimzqca.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gtyfffyppk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj202588.top/gtbmiyipyf.html

[Q43] 标量子查询
来源：http://hz.nanxuanxn.top/gtoebllwgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtgstgepln.html

[Q44] IN 子查询
来源：http://hz.yuxming.cn/gtdsdzyiri.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtzanekdue.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gtihswisoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtchznpfdn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtjyqodixw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtvqmblyxi.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtvxpzuqgr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtpytbhaim.html

[Q48] CTE 公用表表达式
来源：http://hz.svipenyu.cn/gtiuytwqnb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtrvpnlivx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gtsulnhtut.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtgekasvsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtqiuxyrft.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtawixysfb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtfwtkecuc.html

[Q51] 用子查询更新
来源：http://hz.sufxvd.cn/gtebcrpzux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtpfmohich.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gtjjhpldde.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtmyvvotwz.html

[Q53] 按条件删除
来源：http://hz.smart0.xyz/gtbunyygkg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtofegcrjp.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtbbnczkoe.html

TRUNCATE TABLE logs;
来源：http://hz.yvedp.cn/gtlkrgomzl.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gtibqrfqho.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtebcwhwez.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sufxvd.cn/gtbpobpjre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenzaomai.com/gtvaaxsani.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtmbzyqawz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtzzwlmluh.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtdasedryd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nwbrower.top/gtgzpovccw.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gtvqcpvwgx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtidtuntdb.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gtnvkxsexs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtadjygign.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtburxkrwx.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtisiptqxg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtulhjlcgi.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtpukhyxgb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtyakfxelv.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gtmdgyqsve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtfsjbkrac.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtrlatpmmu.html

COMMIT;
来源：http://hz.yueranfly.top/gtqbcuirra.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtbspayurf.html

ROLLBACK;
来源：http://hz.tian-w.cn/gtorrcprsk.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtdwqfmpmz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtptdmtwsh.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtupplqnvg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gttfpyoaad.html

[Q68] 保存点
来源：http://hz.c1oappe.top/gtjorxgdao.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtfbsezfza.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtakczyrfy.html

[Q69] 查看执行计划
来源：http://hz.sufxvd.cn/gtdcdxthbf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtgovdfpsc.html

[Q70] 更新统计信息
来源：http://hz.ybcxt.top/gtohcpgwui.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtrzmxritb.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtlepxvrle.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gttcqfukcp.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtmxofhiaq.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtqauaykfu.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtflpejmme.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtpsdswkln.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtxgziybzc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtfskcuodb.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gtrfmhzwfq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtaipfhplt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtvvolwgbp.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtylrnrjja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.fengsongda.top/gtfzihrsxd.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtvpvcdyyj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gtwuwjmcbk.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtnoxizypq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtzxkvsova.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtloletcji.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtktlcbpjd.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gthymksehf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtfjkfaemo.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtoxkizldi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtujfpssmd.html

[Q82] 字符长度与字节长度
来源：http://hz.jinyuanbaomall.cn/gtrjxccjev.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtklnflmeq.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtwytubrnc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gthamisymz.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtxmrfxvro.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtmcenlpbd.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtkhpyidoe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgufenzy.top/gtyvcztwpx.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtzdvrqhod.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtnnclnwju.html

[Q87] JSON 字段做条件
来源：http://hz.meibo888.top/gtjliyxilc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.quarkkingdee.top/gtyhopymid.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gtatvlqhbz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jiagoushi.top/gterqgwpum.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gtoatsyoiz.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtfhvgolxz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gttnxatddh.html

[Q90] 生成序号列
来源：http://hz.hongshengwenyu.top/gtibymeywf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtggwmvpmj.html

================================================================================
来源：http://hz.nanxinkj.top/gtrksfkrdq.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtjcoaasgf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvgacytii.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtybgziggs.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtxpqlfddv.html

set -euo pipefail
来源：http://hz.wangshuangyany.cn/gtymhewxbx.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtmjdttfqs.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gtswgdsgfp.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtwerkxozt.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtvwqnqqyc.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtslslkzxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtgtsvasoz.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtrcfpemml.html

name="${1:-default}"
来源：http://hz.ywan-chungtsiang.top/gtuqrivltv.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtzaezdbsl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtinefvtlb.html

[R07] if 判断文件
来源：http://hz.jyoumei.cn/gtsujvebtb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtbzkjrcca.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtbgyehyqg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtqxgjhkjl.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtinbgszmg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gtzrwbemif.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtbibdsfjg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhixingplan.top/gtmzphhomu.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtalvuhdwt.html

case "$1" in
来源：http://hz.yj20258888.top/gtwdxhslpw.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtzgnmmgrl.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtykwtgwzq.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtchslnnyo.html

esac
来源：http://hz.hongshengwenyu.top/gtltnvbqri.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gtwqxirwwb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtafccderf.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtxzjqakxb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtokccgtip.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtvpkwsvsf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtddcgtrjn.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtvpmazyxr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtxddlmjzp.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtgvqprfnm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtbhwrcdux.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtqunxdaqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinghuilouyu.cn/gtmkwkktsg.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtxzzacamr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gtsqpcuvgs.html

[R19] 数组长度
来源：http://hz.yangfankeji.com/gtczxppsuu.html

echo "${#arr[@]}"
来源：http://hz.iojbl.cn/gtcoufwlfl.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtnthbspju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtgderttfg.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtxgsskcxp.html

echo "${#s}"
来源：http://hz.birdmap.top/gtbzrrpjym.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtmrrxnsvq.html

echo "${s:0:5}"
来源：http://hz.havefunace.top/gtktfyahqj.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gthqysoaix.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gterddbrtk.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtpazepjme.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtzexpuoyp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtvpounrit.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtwkgcqoqv.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtengpdrog.html

now=$(date +%F); echo "$now"
来源：http://hz.guowangkeji.top/gtchgfaiac.html

[R27] 算术展开
来源：http://hz.tianlin.xyz/gtdrdmfrvi.html

echo $((1 + 2 * 3))
来源：http://hz.guannengcc.top/gtwwbsnawz.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtbqaoqpwa.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtzmvynpmk.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtduphmjgu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.c1oappe.top/gtnndouuuj.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gtaubxlmrt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtzwzgmiym.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtgqlvksmb.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtuehlgper.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtfimwvqcj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtlrjmuqgy.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgfzy.top/gtyohybsuz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtpnzzuklm.html

[R34] 退出时清理
来源：http://hz.shzxlz.cn/gtmknjbzfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtdsinlzyg.html

[R35] 后台执行并等待
来源：http://hz.zhiwuduotai.top/gtgsnpmsjf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtnytsfzeo.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangtech.top/gtbhgftiij.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tianlin.xyz/gtncbrgumq.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtzaokbckj.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtfcwsthlb.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtebckdexs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtdbyvkbtk.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtovemtvxh.html

cmd > out.log 2>&1
来源：http://hz.ppjwa.cn/gthhulywfh.html

[R40] 追加写日志
来源：http://hz.sxryk.cn/gtabpdyqvf.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gtfqiltczx.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtyfyereub.html

cmd >/dev/null 2>&1
来源：http://hz.jiagoushi.top/gtcizcqtnc.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gthkhwnnbr.html

wc -l < a.txt
来源：http://hz.zdqjudy.top/gtjcnzuxhk.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gtongmxsdp.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtpmlzlecz.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gtfpudfbiz.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtlquaklmq.html

[R45] 批量删除
来源：http://hz.zhixingplan.top/gtexisrajk.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtrepgdchm.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtevmrmhtj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtcehsytis.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtftvbawsx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gtiywlstud.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtqxdoumyr.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtzmqvxbct.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtbqfcsgnv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gthpojluwt.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtgzxxymyn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtbrckbktg.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gttbrxoqdi.html


<!-- 参考信息 -->