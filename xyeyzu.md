代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtxtryzutf.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtccswbipg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtfbvrbocm.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtyxptxrqr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtjptmnahg.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gttnowdqxy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtraaucrxg.html

[Q10] 插入单行
来源：http://hz.jyoumei.cn/gtxrkpuqcu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.meibo888.top/gtqchjzoql.html

[Q11] 一次插入多行
来源：http://hz.yongpay.top/gtgufpqcvw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cucudq.cn/gtkndjekzi.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gtlvxjpbsy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jianghu66.top/gtwohheefu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.quarkkingdee.top/gtftcglsnb.html

[Q13] 忽略重复插入
来源：http://hz.chenlongwang.top/gtewlrwime.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtqpeifmmx.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtzrpdoubm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxuanxn.top/gtafmikqbk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gttbefkhhu.html

[Q15] 查询全部
来源：http://hz.0kj1m.cn/gtllivuxqn.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtexlkagha.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtyejocpbk.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtdgxktbql.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtodifzujg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hysaishi.cn/gtzhkdyydr.html

[Q18] 模糊匹配
来源：http://hz.yonumen.top/gtnfpwjnam.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtpnjfuxsh.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtzswerggz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtfydrmeih.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtczyuotar.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxuanxn.top/gtgezdjwis.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gtrmslmosk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jiagoushi.top/gtcifbtxgu.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtfwttqmqb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtsydcltbf.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtwhzehwew.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtlbxidfhh.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtceofarak.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtcobwpkjl.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtfssvqkat.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.haohaochexian.top/gtijhtlivf.html

[Q26] 计数
来源：http://hz.pycfn.com/gtymjhssmb.html

SELECT COUNT(*) FROM users;
来源：http://hz.dianchejie.cn/gtzahtonfb.html

[Q27] 条件计数
来源：http://hz.svipenyu.cn/gtndplsluk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtcbqqhxwv.html

[Q28] 求和与平均
来源：http://hz.kuanghao11.cn/gtldqmmafj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gogol.net.cn/gtirvmfgnc.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtaukvaksy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydjk.org.cn/gtggruyidq.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtucfqwtpw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtxnzbgjpm.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtshsddgon.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtuitlrton.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtvojxupwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtkksfyhgg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtzfpkpcgq.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtjyuhqsrg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenjidiqi.icu/gtqjgstzlc.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtuesxzjzl.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtbhhzvuio.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.feifeiyinyue.top/gtbqajxyma.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtzjlomlli.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtofjjiszw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gttiafzirb.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtxlzhzyno.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtwpxlprtq.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gtjohwbtqu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnqzz.top/gtomcqefqn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtrcyibolq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxinkj.top/gtdwaatsza.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtkponczvm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtilnfpqoz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtbcexinnu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtqdnkblfj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtzwkpuavy.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtehoyhurz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenlongwang.top/gtejiyxjcn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gtxujysxab.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtlssujvcv.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtcsiatgke.html

SELECT u.name, o.amount FROM users u
来源：http://hz.snrcjt.cn/gtpfbupjuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gthlgenqqy.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtkqdkosxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gtvksnckos.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtmyhrlkia.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gthetfjtld.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtscaavohe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtxtfcilqb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtodnbdsrd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtywtptafy.html

[Q47] 与平均值比较
来源：http://hz.redwolf501.top/gtzdlwmqoy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtmwatxrdz.html

[Q48] CTE 公用表表达式
来源：http://hz.xylfe.cn/gtgiczynla.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtujyosocp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtqqhpyyvy.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtfwgmccil.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gtdcyehequ.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gthaarxxfg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtsdjcovqt.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gtvkhddtxf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtvlvsjxci.html

[Q52] 删除指定行
来源：http://hz.xinyue.icu/gttwervbpk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtndqekxms.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtykoslcpu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daria6918.cn/gtstpectpg.html

[Q54] 清空表
来源：http://hz.chenjidiqi.icu/gtamrobutx.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtubizrflt.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtofrzvjuc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gttmdcwzfi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtyhriuyvy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gthmhgikfv.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtgjwotion.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pengpengdd.cyou/gttjfrvsbi.html

[Q58] 累计求和
来源：http://hz.fengsongda.top/gtfhaabrcy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtifsxhlyn.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtefnosqzv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtialwtzvl.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhixingplan.top/gtlzuumydl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtvjjdyffo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuxming.cn/gtwthpfcgi.html

[Q61] 移动平均
来源：http://hz.nwbrower.top/gtmxbbnjkw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gtsbwnyhdi.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtulwecgwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtftoupcfo.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtgkhgjpoi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hfpthk.cn/gtlakjnvkw.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtkshkumda.html

COMMIT;
来源：http://hz.tianlin.xyz/gtlhqaipit.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtumjqkhqz.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gtplmxwkcd.html

[Q66] 行锁查询
来源：http://hz.zhoulong.xyz/gtlibugjos.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gtbatqylnd.html

[Q67] 设置隔离级别
来源：http://hz.gotoacloud.top/gtfzzfrqym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtlfmqwagu.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtdsgswmvp.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtkwelcpgj.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtbhldeqpl.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gttyaatqrz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dianchejie.cn/gtosppeurj.html

[Q70] 更新统计信息
来源：http://hz.nanxuanxn.top/gtypzmfcit.html

ANALYZE TABLE users;
来源：http://hz.pengpengdd.cyou/gtnmugbley.html

[Q71] 查看建表语句
来源：http://hz.yj20258888.top/gthsgqipsq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtotiriypl.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtnvjtoyjl.html

SHOW INDEX FROM users;
来源：http://hz.chenlongwang.top/gtlcecvfhq.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtfslwkbcc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtorypyxxe.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtmjbmnsfp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gogol.net.cn/gtrojfilss.html

[Q75] 日期格式化
来源：http://hz.hysaishi.cn/gteftfyhch.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtxoxkocwd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gthbaemynk.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtbykdkqzp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhijiandao.cn/gtomlcbkow.html

[Q77] 时间加减
来源：http://hz.guowangkeji.top/gtdoncslem.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtxogopbxn.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtnqtqrbwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gthxqkedow.html

[Q79] 字符串拼接
来源：http://hz.shuidangran.top/gtceavgpli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtgddpijzv.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtbnozalbs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtrbcqfqer.html

[Q81] 字符串替换
来源：http://hz.cashguo.top/gtlwxmlmwk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtjcyvwasy.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtzexgdmzo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtqcsnrpbs.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtwjqomdpc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gtxeakiowz.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gteplayjnp.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtiyzubcnd.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtrfmdaljw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtylkhylfr.html

[Q86] 读取 JSON 字段
来源：http://hz.c1oappe.top/gtmwtunzaq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtuiwvdsva.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtcyyoipcv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gthahsugxy.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtlgkmdqby.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gtfxomybdc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtnbnueksb.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtcrpxyxjf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tanke756.top/gtvkfdpcdu.html

[Q90] 生成序号列
来源：http://hz.sxryk.cn/gtilkoynzy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtxftjivve.html

================================================================================
来源：http://hz.fzhhl.top/gthzeabpbd.html

R. Bash 专题
来源：http://hz.hnqzz.top/gtgtejmkoc.html

================================================================================
来源：http://hz.mhx1999.top/gtrkuufxba.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtbohexvzb.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtgvdmjzkf.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtvmkgrbji.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtnhxcgpku.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtjpiwbkhj.html

[R03] 只读变量
来源：http://hz.hongshengwenyu.top/gtmdyfhsvi.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtcitsijkh.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gttqnysefp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hongshengwenyu.top/gtqpvbcnlc.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtcmuzdvje.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtiumjlops.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtrporffqx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jiagoushi.top/gtakdehibl.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gtvddawmgl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gtlksspjsy.html

[R08] 数值比较
来源：http://hz.gzhubu.top/gtxeqxbixt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.meibo888.top/gtduiachmp.html

[R09] 字符串比较
来源：http://hz.jlsjyb.cn/gtvwpucsgh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtmazopmdz.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtszagceap.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangshuangyany.cn/gtfpcolwpw.html

[R11] case 多分支
来源：http://hz.tian-w.cn/gtnggaoiwr.html

case "$1" in
来源：http://hz.jqgfzy.top/gtzegzzoag.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtqcpbbauk.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtchhqpzij.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtvainijbm.html

esac
来源：http://hz.hysaishi.cn/gtyucztohg.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtpkphkjnu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtwxjylups.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gttcmuafer.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gttlzldbao.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtehkjqvle.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aizwys.cn/gtpzvbbzvt.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gtqabrurae.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.vqdsnc.cn/gtlgzzqhfu.html

[R16] until 等待条件
来源：http://hz.shuidangran.top/gtzrglmagz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtllzeubgw.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtfgyooqoj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtcoymmspy.html

[R18] 遍历数组
来源：http://hz.sysykeji.top/gtfvihmfia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gtpfwcmmay.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gtxykplaqa.html

echo "${#arr[@]}"
来源：http://hz.sweek.top/gtnqvcrcpg.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gttmcbscns.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtsyfxjxjm.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtzglvizpg.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtgzounpga.html

[R22] 截取子串
来源：http://hz.zhixingplan.top/gtwtgxdeke.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtdubndypt.html

[R23] 字符串替换
来源：http://hz.aibaodan.cn/gtgegfhbww.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtgoeicxci.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtoarzvhtf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtzuwymnyl.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtjyldxpim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxinkj.top/gtofktopag.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtmhcsskyb.html

now=$(date +%F); echo "$now"
来源：http://hz.zhiwuduotai.top/gtsbzqsuvx.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtflueotyo.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtkeiylewg.html

[R28] 浮点运算
来源：http://hz.jinqigufen.top/gtnfbyqqfn.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhaomingkeji.xyz/gtqhxqcwka.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtkahghcqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gogol.net.cn/gtdwqtlxlt.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gtprdufjsv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtvlpjpzse.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gttexbiazv.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gthkpfuhxi.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtmqlrxsnr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtskujkmbp.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtpvoskljj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuanzhike.top/gttwajsxlo.html

[R34] 退出时清理
来源：http://hz.gaohongyu789.top/gtepjsedej.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtaxydbxof.html

[R35] 后台执行并等待
来源：http://hz.redwolf501.top/gttbqomsfy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtbtmkrzan.html

[R36] 并发执行多个任务
来源：http://hz.shzxlz.cn/gtadjanyia.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtobkzupjf.html

[R37] 把输出赋给变量
来源：http://hz.gzhubu.top/gtfizgvpzp.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtclgudwvx.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtgkdpxjhx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigufen.top/gtdyppefmi.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtyttjkmhq.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtsnxmzjxv.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtfatcbgot.html

echo "log" >> out.log
来源：http://hz.fengsongda.top/gtgmzztqea.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtvuqoxsry.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtfqhhdixx.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtlsuktynj.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gtzswwvepa.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtioddlaln.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gtuzwxupfn.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtuorecckm.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtrnodcmqi.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtvsyrfbsz.html

find . -name "*.tmp" -delete
来源：http://hz.ydjk.org.cn/gtewgeyyqo.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtvbqtqctt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtdlomystm.html

[R47] sed 单行替换
来源：http://hz.xinyue.icu/gtrxqqxhqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cashguo.top/gtvxuawxqo.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtjhryzmfd.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtibxwkvdl.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtevptinwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gtexbdhpte.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtwczvozpz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtixllbpvw.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtxtthcjlu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtvzcugpqp.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gteazcuemr.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtdwsvjuwn.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtpgpjpygt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtsqiqrnxx.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtmaqobitk.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtjwugdkgu.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtxutcjdai.html


<!-- 参考信息 -->