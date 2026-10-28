代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.haohaochexian.top/gteqhwwwmd.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtoyfcehqh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtapssregt.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtcmuinzyn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtwajwvwmc.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gttnpsruru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtmwodqgnn.html

[Q10] 插入单行
来源：http://hz.dashuyun.cn/gtigymenvk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.redwolf501.top/gtcfqkjsqs.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtkpvxkklo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtmhskesje.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtpqmmelsi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtnyfanoyo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtbbwcepvf.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gthewjecrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtblwbfljk.html

[Q14] 存在则更新（upsert）
来源：http://hz.xylfe.cn/gtrvjutceg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtacpfyajn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtndytydnc.html

[Q15] 查询全部
来源：http://hz.yj20258888.top/gtnujabgur.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtgefcluui.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gtsdvmwtdn.html

SELECT id, name FROM users;
来源：http://hz.cashguo.top/gtlkxmkdwv.html

[Q17] 条件查询
来源：http://hz.andypj.xyz/gtvtfukivq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtrxbhbxlj.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtiiprirwq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tianlin.xyz/gtlneelhix.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtkaraetwr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangdashe.top/gtgkijfuji.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtsbypirab.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtanjfnzqd.html

[Q21] 空值判断
来源：http://hz.birdmap.top/gtantaspbb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ywan-chungtsiang.top/gtevycwmyc.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtytyrnrfc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtotwaizuy.html

[Q23] 分页
来源：http://hz.meibo888.top/gtwcwxioff.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtlgezxyte.html

[Q24] 去重
来源：http://hz.ydjk.org.cn/gtyjqqvrxb.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gttyadhxvw.html

[Q25] 只取前 N 条
来源：http://hz.jlsjyb.cn/gtxohpsiyq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtfrjawbwk.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtotftcbna.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtyriuslnc.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gtlnnfmlyx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtccftsjnv.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtgnemabfo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtrwhvdfmy.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gtbcpoqnmd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.redwolf501.top/gtaoghdpoo.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtirlutlii.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtlwrohmxe.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtlddrzdtr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtxyahtbul.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtzyvutfqk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtlfczuong.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtbepafuyi.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtyirzgoim.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtpelbrygy.html

[Q34] 每组取第一条
来源：http://hz.kuanghao11.cn/gtseeyyygt.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtjaowfzee.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuetiantiany.cn/gttcqnezsp.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtquydrupk.html

[Q35] 内连接
来源：http://hz.iojbl.cn/gttneqmnwn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtegxpymtc.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtwijvmnkz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtbmdkohqy.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtjebsplgb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gthkeserex.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yanxiufei.cn/gtwqumxqom.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gtmqkrvcxb.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtsshbvrgs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtpcirgtyl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtovragndw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gtuczggulh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtlxskdvhy.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtbfssedmv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tianlin.xyz/gtkhwwqgeg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gthahmbgco.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.vqdsnc.cn/gtjpoxukbi.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtvsiyvuyb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtiwhznesb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.birdmap.top/gtixrrhpwx.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtunmesslr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtekmofuwg.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangtech.top/gtaitvevxk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gtchhdnoux.html

[Q45] EXISTS 判断存在
来源：http://hz.xinyue.icu/gtqbaoxmjm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtptonkosu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yangfankeji.com/gtxergjqck.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtcpaflovi.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtekyijaxw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtspgdfioz.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gtfawloknx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yangfankeji.com/gtqasdjbjc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shangyingyoupin.top/gtltoxcmwq.html

[Q49] 更新单行
来源：http://hz.quarkkingdee.top/gtajdglswu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.andypj.xyz/gtuydeagxn.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtbvjnwqia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtmgxvpthi.html

[Q51] 用子查询更新
来源：http://hz.chenzaomai.com/gtevdunjyu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtdvgifuid.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtglbkdetl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shuidangran.top/gtuhzltspc.html

[Q53] 按条件删除
来源：http://hz.ivvv.top/gtpjkkofqs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtyqeuvtjw.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtcjkkwpxt.html

TRUNCATE TABLE logs;
来源：http://hz.gotoacloud.top/gtcawloanq.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtoagnwsnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtgiftgnpr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtaatxzqvl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtxoffwzzj.html

[Q57] 行号
来源：http://hz.guowangkeji.top/gthkietpmt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ivvv.top/gtcyscknme.html

[Q58] 累计求和
来源：http://hz.feifeiyinyue.top/gtmpfvmihz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtvzqzbzze.html

[Q59] 分组内累计
来源：http://hz.hfpthk.cn/gtkskuxcfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtduzveeta.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gteogywwbk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aizwys.cn/gtzjnqdsvg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtcmrqsoge.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtwniercgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtxgpdewgo.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtygaaszhj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtsweskyyo.html

[Q63] 开启事务
来源：http://hz.daxiang520.top/gtcbyajlyi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtypulwwlp.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtvohbyjny.html

COMMIT;
来源：http://hz.zhengqikj.top/gtagsdwazx.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gtxqpounrt.html

ROLLBACK;
来源：http://hz.yj20258.top/gtfjmoohjg.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtqbwmsvgo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shangyingyoupin.top/gtszysqwwg.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gtxakxdjmd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtzekcpgjb.html

[Q68] 保存点
来源：http://hz.iojbl.cn/gtfrdncxdr.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtfmwtdihj.html

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtqadvenex.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtgspibslh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtzrlpxmud.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtxbhredcc.html

ANALYZE TABLE users;
来源：http://hz.shzxlz.cn/gtpyhflovl.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gteixqhnoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yongpay.top/gtkydvrgvx.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtntjpegus.html

SHOW INDEX FROM users;
来源：http://hz.nanxinkj.top/gtlcffvjfr.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gtuglnvlmg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shuidangran.top/gtxhvnkhsc.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gthwequoft.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtaomduoza.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtxfymkisf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtwaiurpph.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtbuvkvkup.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtiiyoehdv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gtameczoxd.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtietogrjt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtnvdvkpfk.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtovcfyxfk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtebdqprbo.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gthkyliegk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgufenzy.top/gtypyolthd.html

[Q80] 字符串截取
来源：http://hz.jlsjyb.cn/gtjwwasews.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtfcvsylvy.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtudhzoevq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtgjozbhsj.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigufen.top/gtemeepxul.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtvoljpnba.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtstekttrf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtltxhxppg.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtairuuynp.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gttiakpqcy.html

[Q85] 数值取整
来源：http://hz.xylfe.cn/gtmcfwgwcs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gtfxoljnqh.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtykudlzzn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhijiandao.cn/gtdzihmaxt.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtlydqlkgl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtuxivvshr.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtipentlkj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtytayxaqh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtcxthglqa.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gttdpkkkav.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtmcvliljd.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtgyoqteku.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtiwvwcegt.html

================================================================================
来源：http://hz.yvedp.cn/gtifqncqzv.html

R. Bash 专题
来源：http://hz.gaohongyu789.top/gtcxzszoqb.html

================================================================================
来源：http://hz.aibaodan.cn/gtrzdicgwr.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtjzndpolk.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtcrymoasp.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtgiajhtuw.html

[R02] 变量赋值与使用
来源：http://hz.meibo888.top/gtodwnibhj.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtnblmhdzy.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtiaaenscw.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtqhszzkbn.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtzkkxgsgl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtdlyzrkel.html

[R05] 参数默认值
来源：http://hz.shangyingyoupin.top/gtyrimwvdw.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtejexfbjg.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gteartyhdh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtnpzmwhyq.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtkyvcrklz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtfefnfrqd.html

[R08] 数值比较
来源：http://hz.sweek.top/gtpzfueoak.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.iojbl.cn/gtxskbrwcw.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtjzuivmjs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtjgmazjmc.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gthnrvlaht.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtfptunifz.html

[R11] case 多分支
来源：http://hz.shanyushiyangtech.top/gtcplxcwxm.html

case "$1" in
来源：http://hz.jqgfzy.top/gtphqiekzk.html

start) echo "启动" ;;
来源：http://hz.shzxlz.cn/gtlqkzpybw.html

stop)  echo "停止" ;;
来源：http://hz.cqqwz.cn/gtjcwcjfxo.html

*)     echo "未知命令" ;;
来源：http://hz.jqgfzy.top/gtnmqbrgtd.html

esac
来源：http://hz.sysykeji.top/gtgzdfpwie.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gtefqhswwj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nwbrower.top/gtizzlrcmw.html

[R13] for 计数循环
来源：http://hz.shanyushiyangtech.top/gtephvhtqb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtxelncqwe.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gthkgsgvdj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cqqwz.cn/gtkqaeanvy.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtfxzprtxk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtxiecqryv.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtbdrbpeem.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtzylkpihc.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gtoohrlgnu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xziqi.cn/gtdxicsfsy.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtqabzfbxh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtukfqftcx.html

[R19] 数组长度
来源：http://hz.chenlongwang.top/gtbrfbitai.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtglvczsnn.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtjprbspfd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtozkbadgd.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtfqtsawii.html

echo "${#s}"
来源：http://hz.tanke756.top/gtzvhexhrq.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtsbmifhwf.html

echo "${s:0:5}"
来源：http://hz.yvedp.cn/gtwmblwgia.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtwplwvtjw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yueranfly.top/gtbddhxvpn.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gtxuejyghb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtqnmncnfa.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtrkhsberg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtikpnwegd.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtxojhjdpe.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtkdowiyjs.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtjtnuklxg.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtakrrclft.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtdiyydzgx.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtieaxjmaw.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtlvprtrjb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtvniqnwjp.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtyijrphnu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtrgovohof.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtitvqxaeu.html

f() { local x=1; echo "$x"; }
来源：http://hz.gogol.net.cn/gtbizzwomr.html

[R32] 参数个数校验
来源：http://hz.sufxvd.cn/gtkqoqgeuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gtjaikrzrs.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtzqpadvzj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtrgqvvkmb.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtcfujhyaa.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gthcwolacr.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtkwguihyk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtunuevxax.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangtech.top/gtvoecgaiu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtyfuzlxvk.html

[R37] 把输出赋给变量
来源：http://hz.yj202588.top/gttvbqqsed.html

files=$(ls -1)
来源：http://hz.shanyushiyangtech.top/gtjpmnxcwj.html

[R38] 管道串联
来源：http://hz.xinyue.icu/gtnppcpbvu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtiexvhjpq.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtfsbfpoje.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gtcukqwqaq.html

[R40] 追加写日志
来源：http://hz.wangshuangyany.cn/gtahfvcypg.html

echo "log" >> out.log
来源：http://hz.sxryk.cn/gtcaemagqc.html

[R41] 丢弃输出
来源：http://hz.jyoumei.cn/gtbuhkrxdz.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gtbzznnqjb.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtjkykjbme.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtiwtneatk.html

[R43] 按名字查找文件
来源：http://hz.fengsongda.top/gtpouqokor.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gtlivnosep.html

[R44] 按修改时间查找
来源：http://hz.xylfe.cn/gtmarukwwk.html

find . -mtime -7 -type f
来源：http://hz.jinqigufen.top/gtuhcyobxa.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtoaawfrkv.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258888.top/gtdtzuopxl.html

[R46] 递归替换文件内容
来源：http://hz.shangyingyoupin.top/gtblrrozsx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtairlwkve.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtrrgndwou.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgfzy.top/gtdaynlmyx.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gthvzqqakt.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtwdmeukqc.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtoxtergea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtknszhiov.html

[R50] awk 求和
来源：http://hz.ydjk.org.cn/gtnydtboyz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtexjmtbcc.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gtdboxltvv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gtnsksslat.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtihbnolhf.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtufsdasoh.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtcuiznxto.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtsmgkxtop.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gttrcbjczy.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtllpmjbzq.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtnzmmsmmi.html


<!-- 参考信息 -->