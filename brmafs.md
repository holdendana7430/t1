代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pengpengdd.cyou/gtmmlpjzeg.html

[Q05] 重命名列
来源：http://hz.dashuyun.cn/gtijeqhjyq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sweek.top/gtvsuytvte.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtmddymfur.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gtzpszyxyr.html

[Q07] 删除表
来源：http://hz.yj202588.top/gtnbmkpfqv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhijiandao.cn/gtazzsgvhq.html

[Q08] 创建普通索引
来源：http://hz.gogol.net.cn/gtzctncaom.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtezoutoja.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtjklofhuu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtsxuzwhac.html

[Q10] 插入单行
来源：http://hz.shuidangran.top/gtdgenphtr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtmpgsheza.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtobsdbxou.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtapvxadsd.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtpaucanai.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gtxnjgiitg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtoksemfft.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gthezwcdnf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gtikkpkspg.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtgbzsmztd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtccwqkxyr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtwtwmjkfl.html

[Q15] 查询全部
来源：http://hz.dashuyun.cn/gtjbsbyuwz.html

SELECT * FROM users;
来源：http://hz.shuidangran.top/gtqcldvddt.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtmlosjtgp.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gttbgsrfal.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtrcpcfvbf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtzpgjecfl.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtueupwsgr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtuqcvqzqu.html

[Q19] 范围查询
来源：http://hz.hnqzz.top/gtqdbjsbeh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtznbilvbo.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gtmamvkksr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtwitwdwki.html

[Q21] 空值判断
来源：http://hz.fengsongda.top/gtidlbezpc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtsaiygmdf.html

[Q22] 排序
来源：http://hz.yonumen.top/gtpjfatpxn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtchhhakzq.html

[Q23] 分页
来源：http://hz.cheryme.top/gttoptynxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gtdrspiclp.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtiyfauxtl.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtqzdzynxh.html

[Q25] 只取前 N 条
来源：http://hz.c1oappe.top/gtdrzogyin.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guannengcc.top/gtqmyumrvc.html

[Q26] 计数
来源：http://hz.jyoumei.cn/gtvgektozp.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtcmopmphi.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtliasoccy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtuyvwagva.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtselmydgn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtalteicxh.html

[Q29] 最大最小值
来源：http://hz.c1oappe.top/gtvfiusmrb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sufxvd.cn/gtdzhzmmjm.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtibyahevy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtpswjttbm.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtknlzkqzt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtiiaduoun.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtqldvmaah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtdtvvpnia.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtktmbuvzz.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtypxeuusq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtdczgybxy.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtdcqxcsju.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtezszagcs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xuetiantiany.cn/gtalmbeawa.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtcueigrtu.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtzakaleln.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtcoatesas.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtsujbcpfr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtwohdhoii.html

[Q37] 右连接
来源：http://hz.yj20258888.top/gtxsazbfkq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gtfhppkonx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtbwhjuqzt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gtybdkvchm.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtssjovvzv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuetiantiany.cn/gtgkoqfcwf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gthzxlvujw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gtzphyerwe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtowkjniaq.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gthkfgzzoz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gtylrudmwj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtlchjtkug.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtimdvhbwp.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtthwkzjnb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtfkqqybkk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtgosfmfwy.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtnnuukfnk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258.top/gtxabdtqoj.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtjwdtygrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gtohdyyqui.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtbeajapcp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtlruckjjn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhiwuduotai.top/gtghzgyzdj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtpfohqvrf.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtkmireodw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gteyatqmud.html

[Q48] CTE 公用表表达式
来源：http://hz.zhongyouzk.top/gtqfsauqkj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtcviabqrw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sweek.top/gtblynhasv.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtonqvidvo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtcsfxofgd.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtxhljzwxs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtorlcmscq.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangtech.top/gtvgezaoqy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtwdejbgvm.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gtfpclpcfm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtmrbugynl.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtfgnpfpkt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtsmseazfq.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtfjoyfleq.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtlsmefcsv.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtfclwalzj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnqzz.top/gtwkaxuvsv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtaytzmkwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtgyrsgeep.html

[Q57] 行号
来源：http://hz.tanke756.top/gttexldzyu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtomktyabc.html

[Q58] 累计求和
来源：http://hz.wangshuangyany.cn/gtudbbvuhg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cashguo.top/gttkcqycsd.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gthwzfkeet.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtohhyaiil.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangshuangyany.cn/gtrxxgkkuv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtpnnihkrg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtgxrtrczm.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtvgnfmrsd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtcytvsoim.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtxgmijgpx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtzwewbcuj.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtlwmyqfgl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtirfmcdcs.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtjwrpjekq.html

COMMIT;
来源：http://hz.zycfv.cn/gtwbfxvjie.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtpowsfvzt.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtcwgugouy.html

[Q66] 行锁查询
来源：http://hz.52xcode.cn/gtuqhbmddr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtwbtrzdml.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gtmwnidwmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtxrhlcsdl.html

[Q68] 保存点
来源：http://hz.fzhhl.top/gtufhsmrll.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtfkejsbyg.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtpqwpomut.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gtkccceddz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtsmezdhjf.html

[Q70] 更新统计信息
来源：http://hz.guowangkeji.top/gtdytnibam.html

ANALYZE TABLE users;
来源：http://hz.yanxiufei.cn/gtjsynqsrp.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtbgdbswte.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtqpscelrx.html

[Q72] 查看索引
来源：http://hz.xuanzx.com/gtafqzvbcr.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtobftjmqp.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtppbxbywh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gthbtbhqnp.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtdzzueltd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtbqupmjsb.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtmwbnihix.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtbfrhowvh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtngfgtcjk.html

[Q76] 按天统计
来源：http://hz.ywan-chungtsiang.top/gtzwnduldi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pengpengdd.cyou/gthhgpgaym.html

[Q77] 时间加减
来源：http://hz.nanxuanxn.top/gtzzeylvsn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtlozftunb.html

[Q78] 当前时间
来源：http://hz.xziqi.cn/gtgqyrtusa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ppjwa.cn/gtwewmxkpj.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtoetwpruz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtiwghusso.html

[Q80] 字符串截取
来源：http://hz.jinqigufen.top/gtpfvgjddz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtdvfomcia.html

[Q81] 字符串替换
来源：http://hz.mhx1999.top/gtlgkbslgs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtdazvrhyi.html

[Q82] 字符长度与字节长度
来源：http://hz.iojbl.cn/gtintezccb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tianlin.xyz/gtcqrmdzfw.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtembiuvxq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydzc1.top/gtwifritcp.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtmgnxaema.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gttondvann.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtelofdpjn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtlgwhonyn.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtdadtgrkh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dianchejie.cn/gtjgqqvuio.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtuwdzxmry.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtzolzpfah.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtxykyyezy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangkeji.top/gtlaunwjcf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gogol.net.cn/gtroavgijp.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtobhjkdte.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtiswhzuek.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtshqiampe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtzagknmgj.html

================================================================================
来源：http://hz.52xcode.cn/gtarssdiyi.html

R. Bash 专题
来源：http://hz.yj20258.top/gtjzidsyda.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthkwfckgv.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtvtjdxglv.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtinknylwt.html

set -euo pipefail
来源：http://hz.jqgufenzy.top/gtgdigeser.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtqylxeass.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtrgisqfly.html

[R03] 只读变量
来源：http://hz.sysykeji.top/gtixjcxdcj.html

readonly PI=3.14
来源：http://hz.yanxiufei.cn/gtpgiabogj.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtechwrljg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtcozfjymf.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtrqxcavii.html

name="${1:-default}"
来源：http://hz.sweek.top/gtingpfvcl.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtnttrfuxb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tian-w.cn/gtgurdrrvh.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gturqbuylb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtlydqdcug.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtfedtdfse.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtpapgibmm.html

[R09] 字符串比较
来源：http://hz.hysaishi.cn/gttxzmviwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtyhuxsanc.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtbstlnsjm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtezlmedvg.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtyfwvqhjx.html

case "$1" in
来源：http://hz.xuetiantiany.cn/gtobdomuxd.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtkpxryyci.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtltbcynhs.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtlyymvybd.html

esac
来源：http://hz.bjfxy.top/gtjuqnchgi.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtowmgcwhi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtiwcuiqph.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gthhtakxcw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtrmvnyxde.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtjlckpjlp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fzhhl.top/gtmldtlocg.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtqadcufuc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtxnprouss.html

[R16] until 等待条件
来源：http://hz.hammf.cn/gtuzkfpazh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtnmmpzdjz.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtifrekbgk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtppmczzbf.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtofixzvuq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yangfankeji.com/gtzfhkapui.html

[R19] 数组长度
来源：http://hz.zdqjudy.top/gtjycikurc.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtjfcqvnrd.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gttebmzfnw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.feifeiyinyue.top/gtoolzlcav.html

[R21] 字符串长度
来源：http://hz.dashuyun.cn/gtremlovox.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtrsjnwpal.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtkoovpwje.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtparvjsix.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtxehyxlkj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.redwolf501.top/gtdgzjhnyq.html

[R24] 大小写转换
来源：http://hz.hnxiangtu.top/gthiliriyu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtulyxwnpc.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtawkmxosg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtfecsdagr.html

[R26] 命令替换
来源：http://hz.0kj1m.cn/gtatqqlkpo.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtxalpfwud.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtkdgjzzzm.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtxjehlxdt.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtjvfwwxvo.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtdgmztiuh.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtbjjzksak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.haohaochexian.top/gtvtcbqyyt.html

[R30] 函数返回状态码
来源：http://hz.9152youxi.cn/gtgwchbskw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtpvfvfqyp.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtlxfedktz.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtrcdgnabx.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gtkowwxbfz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuanzx.com/gtsrtmmbzq.html

[R33] 捕获错误并提示行号
来源：http://hz.zhongyouzk.top/gtfxbczgbp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtujqmrrjg.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtxqpuzwjz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gttmvwsdhv.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtepcxgnxv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtiqwkkzrb.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtkwjnvbxx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtqggfmxpw.html

[R37] 把输出赋给变量
来源：http://hz.jlsjyb.cn/gtihdkvgzp.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gtfdkokbid.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtqymjnunt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtkyohwtzo.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtfyvjyjdz.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtdsennbpr.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtctumbfcb.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtmbbqtcyt.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtehxgyfaq.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtghczhtkq.html

[R42] 输入重定向
来源：http://hz.hywenlv.cn/gtrmmqmidf.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gtvwbnqewi.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtuaatvtaf.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtkalghmaa.html

[R44] 按修改时间查找
来源：http://hz.52xcode.cn/gtafiixwhr.html

find . -mtime -7 -type f
来源：http://hz.shzxlz.cn/gtkxkxbibs.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtsfpoqdoy.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtyqacjozt.html

[R46] 递归替换文件内容
来源：http://hz.xinyue.icu/gtsrmnbwsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuetiantiany.cn/gtyfsfywnt.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtucrptujd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtjideevun.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtrtxibgaf.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtsatsxwtd.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtymitqjgi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtikvcthuu.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtzwoqnvoy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtdatmorma.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtsijxoefm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtsvwcjkoi.html

[R52] 统计行数
来源：http://hz.xuanzx.com/gtvecnmovk.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtxiiqmogd.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtbusfpmwk.html


<!-- 参考信息 -->