代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gtpzkubstd.html

[Q11] 一次插入多行
来源：http://hz.jinghuilouyu.cn/gtbgmteumy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtalpifigq.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtjpdjktab.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtifsljedp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gtsqvhmwcl.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtwyrbjilu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ywan-chungtsiang.top/gtigwictue.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtarmjzwao.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtzwlgrneq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gthtrusnrc.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtqtisaoto.html

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtfzeokthy.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtmomxbppa.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gttsjjoili.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtyipionzd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtfvldrdfv.html

[Q18] 模糊匹配
来源：http://hz.hnqzz.top/gtjvarvosa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.feifeiyinyue.top/gttafckniq.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtpmsjayko.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtfryikati.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtcdkmtfmd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtbpisyzmk.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gtxbexvklv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gtxfhhihiv.html

[Q22] 排序
来源：http://hz.c1oappe.top/gtdmhcrbqn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtyfafugag.html

[Q23] 分页
来源：http://hz.jinqigufen.top/gtahdbqosa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtnxjwnixy.html

[Q24] 去重
来源：http://hz.316326.xyz/gtlbretydf.html

SELECT DISTINCT city FROM users;
来源：http://hz.fengsongda.top/gtfkdqpizl.html

[Q25] 只取前 N 条
来源：http://hz.yuxming.cn/gtksflvasm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtuaykydpp.html

[Q26] 计数
来源：http://hz.hnxiangtu.top/gtrjigngvp.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtzoqtvhiy.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtghwzeyee.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yueranfly.top/gtqejjlddv.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gthebujxan.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtpvcxmfyc.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtzugacwsc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtasnehyow.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gtdnblfacv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtvuqqfzkq.html

[Q31] 分组后过滤
来源：http://hz.chenlongwang.top/gtlykamzhi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtbqndxssn.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtgcxnwjct.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtdkaexbhd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shzxlz.cn/gtudddxvjy.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtddncohyg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gtjabciliq.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtslvqmfne.html

SELECT * FROM (
来源：http://hz.zhixingplan.top/gtjybeluzl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtuadlglww.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtthqjgicr.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtntahvabu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gtakramkkg.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtebjpccwy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtidlcjazr.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gthrufozsi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtohypnmhc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtwaukspkp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtkwthfdfr.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtjjlqfbgf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtigydmsod.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtgpdfnxmq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtrcevyewu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtlixskjvd.html

[Q41] 多表连接
来源：http://hz.zhoulong.xyz/gtojrjiane.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gtgfjahash.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtiojctkah.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtrqlmyonb.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtvtlfhjpt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtmsvvnbdt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtykdlmqta.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtnppupfst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.havefunace.top/gtcfqpgsyy.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtthboswie.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtgjoqsqoj.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gthuyxbjqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtvvhcgyrv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtcqueupts.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtzldcrqpl.html

[Q47] 与平均值比较
来源：http://hz.daxiang520.top/gtuazwzsjl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtmbmdieue.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtatcyksax.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydjk.org.cn/gtcdsbtcjm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinyuanbaomall.cn/gtxkufqnua.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtisibpzfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtyseldwmp.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtgpbuhmhm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxinkj.top/gtvokwiveg.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtfmmjvhly.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guannengcc.top/gtzrlefegm.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtslpmaixu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtokqgmpbj.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtiifigufq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gtvhyzdfcu.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtomqtxgcp.html

TRUNCATE TABLE logs;
来源：http://hz.kuanghao11.cn/gtdaycpuxx.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtktboedjy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtabuqscok.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtynowcmde.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtiyetqdba.html

[Q57] 行号
来源：http://hz.hfpthk.cn/gtekvxkwvk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtcjogslnh.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gthgugprsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhengqikj.top/gtifrnxdvu.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtpajqnkpg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtueetfpul.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtipjzsirg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gtzdvateir.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxuanxn.top/gttsfluzig.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtbjftupkv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtdlktoqqj.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtneqjnfay.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gttmuivysq.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtiitsrakd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtdbejlrun.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gtbralzttq.html

COMMIT;
来源：http://hz.svipenyu.cn/gtudkvwxyn.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gttbpuefyy.html

ROLLBACK;
来源：http://hz.guannengcc.top/gtyzviytxn.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtwqujalqb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hfpthk.cn/gtbtfyzozy.html

[Q67] 设置隔离级别
来源：http://hz.fengsongda.top/gtueicfnzs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.birdmap.top/gtqbjwozxm.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtvybnkelg.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtdpxdszjf.html

ROLLBACK TO sp1;
来源：http://hz.hnxiangtu.top/gtfmicvnnl.html

[Q69] 查看执行计划
来源：http://hz.yanxiufei.cn/gtfefpgavj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gteodlfdan.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtllxezexq.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtkfmcsbva.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gteysykmep.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxuanxn.top/gtzekgpyzt.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtgityoals.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtzmhjcjql.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gthbydmxry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhiwuduotai.top/gtpfolwpke.html

[Q74] 强制使用索引
来源：http://hz.shangyingyoupin.top/gtwntmfvgj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtpkvzxrry.html

[Q75] 日期格式化
来源：http://hz.zhixingplan.top/gtruriemfd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hywenlv.cn/gtcxllwqsr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtqlvmsejn.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtijuwgsix.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtxbursfbu.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtxmcpalyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yanxiufei.cn/gtfhsdjbca.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtoosoples.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtapfdqrdj.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gtbfbrqgcl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gttrvkcnhq.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gtntwhkyfy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtbpgfpgvk.html

[Q81] 字符串替换
来源：http://hz.yj20258888.top/gtfhldtzkv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guowangkeji.top/gtydeygity.html

[Q82] 字符长度与字节长度
来源：http://hz.jiagoushi.top/gtvcxlhvyg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtdosyapyi.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtdfpjhkwf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jlsjyb.cn/gtmwylhiwc.html

[Q84] 去除首尾空格
来源：http://hz.svipenyu.cn/gtrkofgigj.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtoztjkmkr.html

[Q85] 数值取整
来源：http://hz.chenlongwang.top/gtaccxvihr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtynfremlz.html

[Q86] 读取 JSON 字段
来源：http://hz.sweek.top/gtpegsombn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gthxyaeztd.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtvoxffndr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtzftcqwdr.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtfccxqorl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gthajitqqe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtosqalfyu.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtetsnxjtq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtimeyiqbl.html

[Q90] 生成序号列
来源：http://hz.bjfxy.top/gtcuxvrybl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gteuinnvxr.html

================================================================================
来源：http://hz.tian-w.cn/gtzkprlwty.html

R. Bash 专题
来源：http://hz.cqqwz.cn/gttmfzmpma.html

================================================================================
来源：http://hz.ppjwa.cn/gtpohcwyqq.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtgxnldiiz.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtlxjbyczv.html

set -euo pipefail
来源：http://hz.cqqwz.cn/gtqdnoiktx.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtbjjnfvom.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gthrkewawu.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtaqrigwxx.html

readonly PI=3.14
来源：http://hz.sxryk.cn/gtjzvstwwj.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gtzittzmih.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtvoyzxqyi.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gtkskijnsn.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtkbpnxrgk.html

[R06] 判断命令是否存在
来源：http://hz.ybcxt.top/gtikiedezd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtzkytnjxk.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtgostkgxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtogmtthcl.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtuakhjzff.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtlnwuauui.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtktovbiew.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtgpdvfynk.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gtcuxmdwli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtolrvpifm.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtcsiugurp.html

case "$1" in
来源：http://hz.fengsongda.top/gtgqgrrxdd.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtnchgialn.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gttjdtsktp.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtvvqhpmon.html

esac
来源：http://hz.xuetiantiany.cn/gthnsugskz.html

[R12] for 遍历文件
来源：http://hz.bjfxy.top/gtapzalare.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtyctpwgrp.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtorbwgedz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gtutwcppzh.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtzuckouqp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fzhhl.top/gtmiaxwtxl.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtnrfwsnxs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhijiandao.cn/gtgdxmnkaf.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtlbgcuhkn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtdhpaeebf.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gttqazlyqz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gtcjxyefoa.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtvmbssikw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtsvoyxkqg.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtuzrknmgb.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gtkguojygj.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtufkmqluv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gaohongyu789.top/gtzcaamkrl.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtghojkbos.html

echo "${#s}"
来源：http://hz.cashguo.top/gtpxrenlma.html

[R22] 截取子串
来源：http://hz.haohaochexian.top/gtfadvcjcr.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtkrtvcluf.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtecvxvdvi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yanxiufei.cn/gtyzzsaxda.html

[R24] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtxomxyejl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtiygeilnb.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtocmkehga.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gttlpjyxdm.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtxukgmfvf.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtrzyktubm.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtivnnevdo.html

echo $((1 + 2 * 3))
来源：http://hz.zhengqikj.top/gtbmbiqnfr.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtsiozvdmm.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gtpjpfedch.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtbymqgrmx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtnptpkyba.html

[R30] 函数返回状态码
来源：http://hz.svipenyu.cn/gtfmfwktjf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ehwqpu.com/gtpcskoqis.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gtyywaaysj.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtasctpcsm.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtnjkftrki.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.c1oappe.top/gtydhbesja.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gtyzevtjpk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gtwwqjwmys.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtmmqjlahx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtafiveloc.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gttmcxwyvl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtdfxezfip.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtubbfxflu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtfwahrotf.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtcjqtiqxy.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gthwzegllz.html

[R38] 管道串联
来源：http://hz.chenzaomai.com/gtpidxlhpu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtdibksseo.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtzoqlerlb.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtiwkinniu.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gtpprqbrnw.html

echo "log" >> out.log
来源：http://hz.xuetiantiany.cn/gtduzuecfj.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtzwyagatt.html

cmd >/dev/null 2>&1
来源：http://hz.hfpthk.cn/gtcrkagtfg.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtgzkofmpu.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtnsneawrw.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtkakdmlzs.html

find . -name "*.log" -type f
来源：http://hz.9152youxi.cn/gtiqczmqia.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gtustqioze.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gthjvgjhnj.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtrfycjhfc.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtizefjhvd.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gtimdebudb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtoegkthqg.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtmajoujot.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.svipenyu.cn/gtkqvdlfoi.html

[R48] awk 取指定列
来源：http://hz.iojbl.cn/gtvfqzemhl.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtxfxeoues.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gtqozkhzbp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtxouxjqkg.html

[R50] awk 求和
来源：http://hz.wangdashe.top/gtunlkbezt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtrnuiiock.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtqogzzpaq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtntqtvyfr.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtincsaecc.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtxffcnmia.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtxoqgizgt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ywan-chungtsiang.top/gtlkoipprm.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtlwxffpqh.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtlpkkgbrs.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtxbekwsgp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtfyrpmxkj.html

[R56] 远程拷贝
来源：http://hz.kuanghao11.cn/gtymlrtiey.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtgnmdbccn.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtueecvvyn.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtyqtlpioy.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtsxqvpvyv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtefcconrk.html

[R59] 发 POST JSON
来源：http://hz.haohaochexian.top/gtznrbkrod.html


<!-- 参考信息 -->