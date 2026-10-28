代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtcotyantx.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gthusejdxv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtedfjgtrf.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtpjoishfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtgzftbuwj.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtwaegodwa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ehwqpu.com/gtvrdsqgof.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtjyrjivim.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtgymxjwuc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gtsevcqexb.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtzyfibemz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtwozwrqye.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258.top/gtgbklauzz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guannengcc.top/gtkcidbgxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtyqdrkdrw.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtiiviujda.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtshfodsgz.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtyderapbd.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtdgzjadpj.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtbssvqhyg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtydmvahlj.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtzulmqtgu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtmqamgtuh.html

[Q19] 范围查询
来源：http://hz.jinyuanbaomall.cn/gtwhultanb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gaohongyu789.top/gtwpxcwoyi.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtncbahujq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtkfqldxos.html

[Q21] 空值判断
来源：http://hz.zhengqikj.top/gtbjebknjd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtzpyvpplq.html

[Q22] 排序
来源：http://hz.tanke756.top/gtikjheyer.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtutsofxpx.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtdpkwlkia.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhongyouzk.top/gtanmlwwop.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtbzkpovqq.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gtlbejoeqh.html

[Q25] 只取前 N 条
来源：http://hz.shzxlz.cn/gtwemruhmc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gticihwdqr.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtajsukajf.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtqofaulpy.html

[Q27] 条件计数
来源：http://hz.jyoumei.cn/gtgylnuhce.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj202588.top/gtyfzwgesj.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtxxyrgzoy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtfdvelvos.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtvxcwpogn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gthxygcman.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtjqbrtfzb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtmlxextak.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gttctimmpu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtjeebhfsd.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtdbvrguji.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtkrjxlafg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtdwuphueh.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtmuuzsugd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtvegyzsyr.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtncxftohq.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtbldmjlgi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtnychiqcg.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtzizxncgi.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtrjfsvjfc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtnflzguxo.html

[Q36] 左连接
来源：http://hz.c1oappe.top/gtjmikmgwf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtypqyzqfb.html

[Q37] 右连接
来源：http://hz.ehwqpu.com/gtsniypdze.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtxypantct.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtosjkgnig.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtxbunkwfk.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtwefkswfl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtvvgnvtwo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtcpimvpxn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtawtbqilh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtogyrvwrv.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtzjddegjq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daria6918.cn/gtahcjedqq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtaocbdxfo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tian-w.cn/gtirmbvwzk.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtugebnwbp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.kuanghao11.cn/gtxbbzzitp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtyujrnlif.html

[Q43] 标量子查询
来源：http://hz.chenjidiqi.icu/gtswudofru.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtvhvvncqd.html

[Q44] IN 子查询
来源：http://hz.wangdashe.top/gtcsidzgat.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtuialbcch.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtqpswetdw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtrkdxitde.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtguiajpjb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtzsutuurz.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtkkpoicwy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtuvwzdkel.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtattklvrr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtzyyzhcxz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtdjpcbdec.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtkoazvyab.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtsomeyuhv.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtqaooptax.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtgujejhsf.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtdcwaiqnh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtnssqsnfx.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtozhoibmb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtrujwmysi.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtlattlaha.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.0kj1m.cn/gtetggtbun.html

[Q54] 清空表
来源：http://hz.gotoacloud.top/gtjxobvwun.html

TRUNCATE TABLE logs;
来源：http://hz.pycfn.com/gtyftdxdho.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtdqsptcrd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtkpoizrwn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jlsjyb.cn/gtqhgdnrxe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtnrkmmxql.html

[Q57] 行号
来源：http://hz.nanxuanxn.top/gtlzolqqff.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtyjbiwdav.html

[Q58] 累计求和
来源：http://hz.jianghu66.top/gtuzzewlqt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtftpjdjuy.html

[Q59] 分组内累计
来源：http://hz.jlsjyb.cn/gtflceqlvn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yuanzhike.top/gtadclsbix.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtcveijpfg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtpyhnjcfh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gtetoqestp.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtlpyllpgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guowangkeji.top/gtirlaonza.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gtgsryhmjr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gthorqsggd.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtbtvorqtu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtuzwzejwl.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtkbzehwex.html

COMMIT;
来源：http://hz.gotoacloud.top/gthfcjwaol.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtdsediegr.html

ROLLBACK;
来源：http://hz.yuanzhike.top/gthuxrgqlg.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtndywtods.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtirnjuzhw.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtyfdlzaxz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.9152youxi.cn/gterbcvtzf.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gthraquwzu.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtdfjldpmr.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtipnvcwll.html

[Q69] 查看执行计划
来源：http://hz.aizwys.cn/gtfnirrgns.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shangyingyoupin.top/gtvqocoazt.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtgglhzdua.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gtyitcnekv.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtkdcetwxj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtbpnmsdwt.html

[Q72] 查看索引
来源：http://hz.ydjk.org.cn/gtbutvqtfb.html

SHOW INDEX FROM users;
来源：http://hz.jyoumei.cn/gtowrcmsmc.html

[Q73] 查看表状态
来源：http://hz.xinyue.icu/gtsxhrarwf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cucudq.cn/gtzjepmxgv.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtutqsvsun.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ybcxt.top/gtglcqougq.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtjbgpjyif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtaqwbpufi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtcnmzduvw.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gthpuxwikz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtgelhwynh.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtjnddmibo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gtdjznqfeo.html

[Q78] 当前时间
来源：http://hz.tianlin.xyz/gthfdpoutr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtvlezoywc.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gthuxdxffn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtiwyzhaez.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtyhgtbywq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtxlyxlbox.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtghshydib.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtmxfevatn.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtxbpxfvnc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gtblvisdfb.html

[Q83] 大小写转换
来源：http://hz.yj202588.top/gtmmtuwqfu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtszyqfgso.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtbwqtqyjl.html

SELECT TRIM(name) FROM users;
来源：http://hz.pycfn.com/gtjklcklzr.html

[Q85] 数值取整
来源：http://hz.cdnleiting.top/gtnhldxxpv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtternyvzv.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtbovsodlz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtibqopugh.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangkeji.top/gtczwnxuhq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gtzfujoeur.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtgtsqnylc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gthdfmhqpq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtajmzxgqv.html

[Q89] 判断表是否存在
来源：http://hz.sufxvd.cn/gtyvfgithi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gthydetzih.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtzstsymzu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtnbfwhutr.html

================================================================================
来源：http://hz.hnqzz.top/gtzvcvpric.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtxqfwzlqc.html

================================================================================
来源：http://hz.andypj.xyz/gtwozvmnar.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtluzjqhcz.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtwztcxaze.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtmsopilzh.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtmiapcwqq.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtwnpwqpdb.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtgufmzmiw.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtjjcvmkcw.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtqltqkpvh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtakbibgyp.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtetofmsno.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtdwbtlplc.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtiveorbdl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtqkgtsuer.html

[R07] if 判断文件
来源：http://hz.gaohongyu789.top/gtusxwibmc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zdqjudy.top/gtxjmyyhti.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtbhqosnof.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtpozinwjn.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtipdvrzpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtfcsqjafa.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtpkuuemat.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtxtaqvmyw.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gtsxxgeztj.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtbhgoyrnp.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtnlzzcdys.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gttxzfwpef.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtzrnitbqj.html

esac
来源：http://hz.tianlin.xyz/gtqlyhsaea.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtanlnrehf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gthcedwudl.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtvkcpevgv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtilnbkjsh.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gtdczypbas.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtkgyneqyg.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gttvjxsrri.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtuunmpjee.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtawstkzyl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xziqi.cn/gttuxohmxp.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtpsgtvgfv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuxming.cn/gtqqozyvrf.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtdvtewtuy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtyltrdmow.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtljbarbxh.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtbwcuqart.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtkvfbynsp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gthkibyotz.html

[R21] 字符串长度
来源：http://hz.kuanghao11.cn/gtohrpeses.html

echo "${#s}"
来源：http://hz.guowangkeji.top/gtcbdgglao.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gtcuymzkkt.html

echo "${s:0:5}"
来源：http://hz.hfpthk.cn/gtnndfchyl.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtcfgimhzm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtabodugtb.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gthlksiwky.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jianghu66.top/gtmqlbucbn.html

[R25] 去后缀 / 去前缀
来源：http://hz.jiagoushi.top/gtngsjbxgx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtwgotmwro.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtsyqfkbop.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtjeljglqo.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtdutwkamf.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtuhoiljuk.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtannzqaox.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigufen.top/gtekhiklra.html

[R29] 定义函数
来源：http://hz.316326.xyz/gtyyvlfejg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ywan-chungtsiang.top/gtwcpxblna.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtkjmoksow.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtmhwwtxmz.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtlllhymyr.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtjcdjhpfc.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtgeytbizx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtzgrxnqdp.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtpvbbgjdt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtkupxivzz.html

[R34] 退出时清理
来源：http://hz.jyoumei.cn/gtcxduwxoz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtxbomejuw.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtgqvdiaxb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtvjmscute.html

[R36] 并发执行多个任务
来源：http://hz.xinyue.icu/gtvfvtyrkn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtaxsoxcrh.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtutbkduiu.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtvjqnmnpc.html

[R38] 管道串联
来源：http://hz.daxiang520.top/gtzxwlugxl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj202588.top/gtaywzxcut.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtrkgyybhn.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtekduyotz.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtdblgwouu.html

echo "log" >> out.log
来源：http://hz.xingfuxueyuan.xyz/gtmgwfsagy.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtsrxxvedq.html

cmd >/dev/null 2>&1
来源：http://hz.vqdsnc.cn/gtdjlxopes.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtubcgpacp.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtcbcggzqn.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtfcbzncxf.html

find . -name "*.log" -type f
来源：http://hz.0kj1m.cn/gtttfmczqk.html

[R44] 按修改时间查找
来源：http://hz.dashuyun.cn/gtnjdxqplt.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtnsazvphv.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtvwkstmtd.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtjjvxpsnt.html

[R46] 递归替换文件内容
来源：http://hz.tanke756.top/gtwfaregjb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtwgtgjneh.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtihrsqtfb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtzjeegqwt.html

[R48] awk 取指定列
来源：http://hz.52xcode.cn/gtlzfdpypg.html

awk '{print $1, $3}' a.txt
来源：http://hz.shuidangran.top/gttmkdqttq.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtdveptuqp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.vqdsnc.cn/gtkfgopqeh.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtwrrarxvq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtgfurqdoi.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtrjofhjoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtjepfwnwk.html

[R52] 统计行数
来源：http://hz.jqgufenzy.top/gtqpwxhdrv.html

wc -l a.txt
来源：http://hz.yonumen.top/gtebxuddcp.html

[R53] 查看文件头与实时尾
来源：http://hz.sweek.top/gtjoekmboa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtmummcibe.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtnfepjyqk.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtxfxepxgo.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtafveedil.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtvawbvgsx.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gttxmcqunr.html

scp file user@host:/path/
来源：http://hz.dianchejie.cn/gtylulobjf.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtkedyxfvn.html


<!-- 参考信息 -->