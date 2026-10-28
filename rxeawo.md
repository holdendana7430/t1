代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtszperjup.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtgmfnhmzr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtqmfgysos.html

[Q10] 插入单行
来源：http://hz.cashguo.top/gtradjfjqb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtmqssfkgc.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtmhubglfn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtotxajpbi.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtbscllyim.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gtbsbrwiud.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtjrefyfxh.html

[Q13] 忽略重复插入
来源：http://hz.yj20258888.top/gtbpxvbsyx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtzduptjqp.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtueeaxbdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gtvqbkzhgb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.birdmap.top/gtwccizomg.html

[Q15] 查询全部
来源：http://hz.yueranfly.top/gtwzdluryj.html

SELECT * FROM users;
来源：http://hz.dianchejie.cn/gtyfhwnkxs.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtwzszumog.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtteyzslms.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtqorwaoul.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guowangkeji.top/gtdjwsanam.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtkgsxbhxh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtecvyhplt.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtchkvyawa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gtqnzotjcz.html

[Q20] IN 列表
来源：http://hz.jqgufenzy.top/gtfuywcizq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtdyneokyy.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtrvursyez.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gtjgjjqslc.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtscdnlqek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtmhgrxgxz.html

[Q23] 分页
来源：http://hz.zycfv.cn/gtgezuvfrh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtuggzqzwj.html

[Q24] 去重
来源：http://hz.gotoacloud.top/gtunpyhpvz.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtxmbfcztn.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gtdfasmazj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhongyouzk.top/gtbeughzuu.html

[Q26] 计数
来源：http://hz.yuanzhike.top/gtrksejbgr.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtnrqcdlsf.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtpxdmiyxt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtcgumofvg.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gthvsjgilj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtvqoevgfe.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtslnydugy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fengsongda.top/gtrmypchpr.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gteikjjykz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtdszswldd.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtasjkcvam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtjgahlgqs.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtxjwqzniq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtymahiuip.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gttctxqswc.html

[Q33] 多列分组
来源：http://hz.hnqzz.top/gtbjucfdqv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtapozoswd.html

[Q34] 每组取第一条
来源：http://hz.cucudq.cn/gtsefwtiip.html

SELECT * FROM (
来源：http://hz.cqqwz.cn/gtpjnkxnmy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtmmfjiijb.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtecdkmzae.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtvdphxctp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtalhgelfr.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtzzazcvpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtumthmomr.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gtnxziahwr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtjflkflff.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtlmtyjkwh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtjisfepkp.html

[Q39] 自连接（查上下级）
来源：http://hz.cucudq.cn/gtqjedqxnm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jiagoushi.top/gtkcglbjjr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtghkqmyen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aibaodan.cn/gtakopmjej.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xziqi.cn/gtbbyajvpg.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtbmuzdmli.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtqssxqwuf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.bjfxy.top/gtuezboqko.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtzsietxmr.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gthplcuihx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtofwrkdvf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigufen.top/gtpcqxqrwy.html

[Q43] 标量子查询
来源：http://hz.tianlin.xyz/gtfznddodv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtuyngfibt.html

[Q44] IN 子查询
来源：http://hz.yuanzhike.top/gtlxztdlnh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtbotrhwxq.html

[Q45] EXISTS 判断存在
来源：http://hz.wangdashe.top/gtmomkkxwc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gttswtzxcx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtprwuuszj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtrkpjlgey.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtvplrqrdh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtqpnlzbsc.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gtcbxdagau.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtzoeygyui.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtzeqculht.html

[Q49] 更新单行
来源：http://hz.zhongyouzk.top/gtrpskstuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtraopxrna.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gthcfnbpox.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.52xcode.cn/gtpgkcndae.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtyegwizqk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtyoiivhxj.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gttvlnljze.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtmckcjrhk.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtgptiaydd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtykglufja.html

[Q54] 清空表
来源：http://hz.jinqigfzy.top/gtygmabimz.html

TRUNCATE TABLE logs;
来源：http://hz.cdnleiting.top/gtuxcyjjjo.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtnjciuctf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.bjfxy.top/gtojnxmahx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtyzvxmmyv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtflaqsmif.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtxwbebytf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yonumen.top/gttnkfbvkp.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtmqfhogpf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.9152youxi.cn/gtaemgrjpm.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtauiahhux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gtaylgtdlu.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtuqveptyq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gtwdzxmkci.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtaxpilqvm.html

[Q61] 移动平均
来源：http://hz.wangdashe.top/gtmarvzpdi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.9152youxi.cn/gtjjztocjw.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtpzqijkrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gterhfmanu.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtvrnaahgc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nwbrower.top/gtikhdczbe.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtcvsccuhh.html

COMMIT;
来源：http://hz.jyoumei.cn/gtwgixbnaf.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gthzvsnweo.html

ROLLBACK;
来源：http://hz.cashguo.top/gtkldvofht.html

[Q66] 行锁查询
来源：http://hz.tianlin.xyz/gtrhsnvarp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gttzmxmlsg.html

[Q67] 设置隔离级别
来源：http://hz.haohaochexian.top/gtdvyjyfvf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gteujbulep.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtbnongcyx.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtbvhzxpfd.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gthmjihdoo.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtretqrizm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtqagyzrdw.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gturrjedob.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtjbqudgal.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtkmvpeoay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtarpixfmz.html

[Q72] 查看索引
来源：http://hz.c1oappe.top/gtmqbaosqg.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtbokzrbni.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtudppeuhd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtirxkgjva.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtnfcdumwp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtbtqqyhkv.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtladtzjpb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtbnceusqb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gttftopisx.html

[Q76] 按天统计
来源：http://hz.c1oappe.top/gtbztwddcn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.svipenyu.cn/gtftiifqrm.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtfzeyjqte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gthxzngynl.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtsdvvmaks.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xylfe.cn/gtfqwwxsyj.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtmmktgqda.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtngeqfctt.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtctlmfpfe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtupvnrcwi.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gtzaxxwaup.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtbwgyodop.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gthyufgzyy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtmcglzcrj.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gtdmvjyosp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtfgbdmnoz.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtukrntvdr.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtlmenkugo.html

[Q85] 数值取整
来源：http://hz.sufxvd.cn/gtrfplyoou.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sysykeji.top/gtlrkwzqdc.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtotmvcdne.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtiobdomjl.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtlplzkwah.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtlroxzsda.html

[Q88] 行转列（条件聚合）
来源：http://hz.pengpengdd.cyou/gtrhzcwsfq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtzjozjkmf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigfzy.top/gtoppeqtau.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtoqznsdjd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtemhfxrfj.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtqbugiamg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cdnleiting.top/gtgqjhlyix.html

================================================================================
来源：http://hz.gzhubu.top/gthcupxnol.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtzmkqhwje.html

================================================================================
来源：http://hz.zhengqikj.top/gtixrodpif.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtmspwfupx.html

#!/usr/bin/env bash
来源：http://hz.guannengcc.top/gtagchqflr.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtjkjedixz.html

[R02] 变量赋值与使用
来源：http://hz.hysaishi.cn/gtstkowrfm.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtlefsjvrm.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gttxfjkihd.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtkidsbsro.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtomrrstjp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtcsaohfcz.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtkuzibzkc.html

name="${1:-default}"
来源：http://hz.chenzaomai.com/gteuvbbimz.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtbnxdzwls.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.andypj.xyz/gttsrbaaru.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtomlybmwb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zycfv.cn/gtcliiqhwq.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtkqlgjmhj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtupmbqpqw.html

[R09] 字符串比较
来源：http://hz.wangdashe.top/gtuzfzwhqn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtgovablpq.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtqerhjsol.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shzxlz.cn/gtnwjluqem.html

[R11] case 多分支
来源：http://hz.yuanzhike.top/gtqxbiciyb.html

case "$1" in
来源：http://hz.iojbl.cn/gtxhdaexuo.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtgsbezpct.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtoevdtpet.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gtgpycxjox.html

esac
来源：http://hz.ydjk.org.cn/gtbktyyfjb.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtsmithfss.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gtvwhbtaav.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtgxhienlf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtjlgspzij.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtcioseiiv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtuvlcqcnm.html

[R15] while 逐行读文件
来源：http://hz.0kj1m.cn/gtzteczcgl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtavfnwhdt.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtpssxcbcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtrdjlilzm.html

[R17] 数组定义与取值
来源：http://hz.gotoacloud.top/gtkowlqgcw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hysaishi.cn/gtpgzwxpzj.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtthqiekjk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtvvpdtzdi.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtwmwveseo.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtrqmfxszi.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtounsotgf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtpbtwoepa.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtqgqgdfzn.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtrsaivkhd.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtdvyahzts.html

echo "${s:0:5}"
来源：http://hz.chenjidiqi.icu/gtkidhbogh.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtvghxdwck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.havefunace.top/gthvwclnzk.html

[R24] 大小写转换
来源：http://hz.yangfankeji.com/gtssylmqll.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jianghu66.top/gtjokxnzby.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtazpwrhyw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtuwcvjcym.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gtsgcbkhwb.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtddbxedbf.html

[R27] 算术展开
来源：http://hz.xziqi.cn/gtnxeguoaa.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtznjmhfvb.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtpuazgixq.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtixhcayur.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtthvrdwam.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cashguo.top/gtsmyhbtor.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gttfizbpqj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gtankvcxur.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtdbunhrle.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtwhabizje.html

[R32] 参数个数校验
来源：http://hz.zhijiandao.cn/gtdtjnzxii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtkpihxlmx.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtpirlyflu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtugcixanh.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtenjlrnty.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtrnsrjltr.html

[R35] 后台执行并等待
来源：http://hz.yj20258888.top/gtotxokhth.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtrlaesboh.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtxvrafrrf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.vqdsnc.cn/gtappyktet.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gtorgmavae.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtrbythhmf.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtlsigvhys.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fzhhl.top/gtfxsaadnp.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtrhxcurvt.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtqcsmigkl.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtcthwalwk.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtsuccsvdf.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtnureyjbt.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtbmztfhba.html

[R42] 输入重定向
来源：http://hz.nwbrower.top/gtysslccvp.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtssuqqrfp.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gtanjxqofh.html

find . -name "*.log" -type f
来源：http://hz.nanxinkj.top/gtzgmrevcp.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtlngrjrxp.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtfwqdsntd.html

[R45] 批量删除
来源：http://hz.yj20258.top/gtqljzvflt.html

find . -name "*.tmp" -delete
来源：http://hz.zdqjudy.top/gtdpbwihlf.html

[R46] 递归替换文件内容
来源：http://hz.xziqi.cn/gttfzhgndp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtzbowutye.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gtnbnclwul.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtqpbqaade.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtpkhgowks.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtsxfnssfr.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtyklndasx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtkyjdwvte.html

[R50] awk 求和
来源：http://hz.jinqigufen.top/gtzyojlkaf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtyajzqhtk.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtlhaslkqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhixingplan.top/gtlnwkgxrz.html

[R52] 统计行数
来源：http://hz.shanyushiyangkeji.top/gtpnrildfx.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtxwxzbtsy.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtsfsyjnyg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fengsongda.top/gtltkpbnve.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtijlvosux.html

diff a.txt b.txt
来源：http://hz.hnqzz.top/gtqnusxgdm.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtklzvsprs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yanxiufei.cn/gtxfxrcfkb.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtyxkhdfdp.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtvokugjqu.html

[R57] 远程执行命令
来源：http://hz.yonumen.top/gtjmarsxnp.html


<!-- 参考信息 -->