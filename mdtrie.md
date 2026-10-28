代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gturawslig.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtcpewyxeh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtvfgqbvwm.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtmiiflbkl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtsnmfgsoz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtpwsxsqbf.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtgpuhmnbo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtuhiimosf.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtxvovmwax.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jlsjyb.cn/gtxagwfxwh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtpliilbhp.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtcqgssluo.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtnrblvjjd.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtyzzhxiff.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtcnkgobed.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtcmiyhhwb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtbgqlyjmv.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtbenwpdnz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtalzmqlkf.html

[Q19] 范围查询
来源：http://hz.yonumen.top/gtvnbtvsmy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cheryme.top/gtpeizhkyw.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtwbgfjtth.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jlsjyb.cn/gtjcqtwbaz.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtihfofjuf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guowangkeji.top/gtjeahpgbo.html

[Q22] 排序
来源：http://hz.cqqwz.cn/gtlkqauvro.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuanzhike.top/gtfiyqklua.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtlilslwvb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtccnhkgdf.html

[Q24] 去重
来源：http://hz.yonumen.top/gtggswrldn.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gtoqntkpzh.html

[Q25] 只取前 N 条
来源：http://hz.yueranfly.top/gtdxcxiggj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nwbrower.top/gtahvmzpjg.html

[Q26] 计数
来源：http://hz.pycfn.com/gtqfdzldzk.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhijiandao.cn/gtcpfoqpoa.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtjtxtitfh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinghuilouyu.cn/gttdhbumza.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtgfieutqs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtdqqoufhx.html

[Q29] 最大最小值
来源：http://hz.aibaodan.cn/gtfdvgshbf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnqzz.top/gtaemsckpy.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtveuglray.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtkctwatjs.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtntcobswx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtrhvzhajl.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtlldzfsqg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtuevezktd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtnvccocvj.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gtwskykrce.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtuhkapclg.html

[Q34] 每组取第一条
来源：http://hz.c1oappe.top/gtqsrcmdmy.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtrgnabfmh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtbnkxclkn.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtlpxdjyfb.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtfjjjerip.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtapkokyta.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gttgjfzfmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtpzxzpkbn.html

[Q37] 右连接
来源：http://hz.sysykeji.top/gtjsnimtsf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.52xcode.cn/gtnexcrdtz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhijiandao.cn/gtaesqhzva.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtwdyeaxzc.html

[Q39] 自连接（查上下级）
来源：http://hz.tanke756.top/gtcntjwrqs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtwyqmptzl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtdyvepdyk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtxafhvclh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtoznriwno.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtjkliglvm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aibaodan.cn/gtdzktdxpq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtnlkfuutp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtxecourvk.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtbzldcgdv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtckhcnxff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtaayxoxzh.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gtuknbbhzf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtahhtdmen.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtuohxlwbb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtuhghhcwo.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtwvvblabw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtglvzcqpt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj202588.top/gtvqmhltnz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtgjsizqwv.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gtvuumxvvi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gtrlksdkul.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gttabveyaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtbjjuhqsd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtrepkpjfs.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtbdheiskf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtgrsotakv.html

[Q50] 批量更新
来源：http://hz.jqgufenzy.top/gtzetlbcuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtcspyqlzq.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtthtzabjr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gttonszrtt.html

[Q52] 删除指定行
来源：http://hz.pycfn.com/gtkepqkrvk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gtxuvyggya.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtygtkctdl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtsxdhvhoc.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtoqajyhol.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtqdzcwhsz.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtlbxegley.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ybcxt.top/gtieuuszak.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtlxcitxdt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtgztzvihu.html

[Q57] 行号
来源：http://hz.zhiwuduotai.top/gtnlmoscsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnqzz.top/gtuuacdieb.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtbrxoprsb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtnyekfgrp.html

[Q59] 分组内累计
来源：http://hz.cqqwz.cn/gtbopovpqh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sweek.top/gthfoikrxi.html

[Q60] 取上一行 / 下一行
来源：http://hz.yongpay.top/gtrwesddhl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aibaodan.cn/gtxkbzajvc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtiqtpdgji.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtfadyqgrq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.feifeiyinyue.top/gtqgzwpdgj.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtzpsghcgo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gthjvynoru.html

[Q63] 开启事务
来源：http://hz.zhaomingkeji.xyz/gthhwuuohm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gtudxhurhi.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtvilavcar.html

COMMIT;
来源：http://hz.meibo888.top/gtocclpbeo.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtfwknmppu.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtqthoxqyv.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtwqsjavtm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtwljhlfrd.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gthihvwcde.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gtyvwqyusg.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gtcobxsouf.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gtniheayve.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtsvokzwze.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtprvootyj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtgxtwickv.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtluxrlrhm.html

ANALYZE TABLE users;
来源：http://hz.nanxinkj.top/gtnhjtkiou.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtmflwbaii.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtahrsumpu.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtxcqqmqxe.html

SHOW INDEX FROM users;
来源：http://hz.jinghuilouyu.cn/gtyqbtahup.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtamsruzcp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtdqhvtupj.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtiwtsjrmu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtpmskntlq.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtnnxcwqht.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhoulong.xyz/gtlpnprxdr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtrgsvatjz.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtspbuipba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtpzdeolcc.html

[Q77] 时间加减
来源：http://hz.jinghuilouyu.cn/gtaoiqznfv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gtahlozdlr.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtbwfouutb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtechheapt.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtaapvbwcb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gthmpqenhh.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtizndvnwe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtdrwomdoa.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtkyxdarmn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtkjqxsjpu.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtbrflpxoq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gtwkapcuil.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtvqfgwgur.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtfziywaau.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtvftnswau.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtmxsrfbxf.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtsmwkqtpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zdqjudy.top/gthgnlkrgw.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gtlgxejcdl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtgfllpltb.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtnkeikmyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fengsongda.top/gtucnzwxib.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtmzztnclz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gttcnxizbf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258.top/gthnvzxrpi.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtunommzka.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtzkxecedi.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtivckwamr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtdxadqxqz.html

================================================================================
来源：http://hz.guannengcc.top/gtxyrfvhvm.html

R. Bash 专题
来源：http://hz.9152youxi.cn/gtgfebmpow.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtidztcnrz.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtdkxcxepe.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gtxagxidah.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtsftqaxrf.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtehlgbekb.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtnxhxfvfk.html

[R03] 只读变量
来源：http://hz.cucudq.cn/gtzmdghpce.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtyzmhuhbt.html

[R04] 位置参数
来源：http://hz.chenjidiqi.icu/gtdsybjwbx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtxtkmumec.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gttrqlddwl.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gthmdmwqaz.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtlnbnyaql.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtwzkoxycd.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtwehqvwws.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtryohhqku.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtpoqiunvx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtaprqltct.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtfkseltsm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtcdnhslcp.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtdsmtoeus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtfugvwrpc.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtvayvmhvv.html

case "$1" in
来源：http://hz.316326.xyz/gtnqpercxp.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtdaqfqjlx.html

stop)  echo "停止" ;;
来源：http://hz.dianchejie.cn/gtvvrxphyh.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtcmtjzpwt.html

esac
来源：http://hz.andypj.xyz/gtrmmwbsvx.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtjqbcltvw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtpxwkyeep.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gtfiptkjyj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gtgzyxmbpd.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtxtnytngj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtirsxbiaa.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gthnprtdjg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtoppgvuwo.html

[R16] until 等待条件
来源：http://hz.ehwqpu.com/gtikgbypnf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gtctgwcijg.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gtwvyyldbc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtbhpwtbdv.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtjbwveprb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gtvtjhpuee.html

[R19] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtkxcvmxxq.html

echo "${#arr[@]}"
来源：http://hz.yj202588.top/gtuyctgqnx.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtkudwwpmu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gthcifzjpu.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtjmguxpbh.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtdilydjpr.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtgdlrkaid.html

echo "${s:0:5}"
来源：http://hz.ppjwa.cn/gtuetkluyt.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtnaarkiyc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtyhzoeobd.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtmpzrhjiy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtvmqdntji.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtvtdaweem.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tianlin.xyz/gthhjdihcl.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtljsgejem.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtucseweaf.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gteacqgmlv.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtxctzqylc.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtcvypuhbe.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtiaqiiihc.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtdqbclcnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhiwuduotai.top/gtfzawikzk.html

[R30] 函数返回状态码
来源：http://hz.sxryk.cn/gtcisdsbll.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sysykeji.top/gtgavqvced.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtdhefllwz.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtmncmzbph.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtriwznzev.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtaxhdounc.html

[R33] 捕获错误并提示行号
来源：http://hz.smart0.xyz/gtqoqdsfjm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gttfjwrgyn.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gthgzqjcmi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtwtgpmfhy.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gtugsuufhx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtzdghyrwz.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtxkrrbclc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtkkoaxxwr.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtbnvcxjgw.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gtrxnukxml.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtpfphqeei.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtbpfrxvzm.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtnzigerkc.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtetfrfgzv.html

[R40] 追加写日志
来源：http://hz.jiagoushi.top/gtdqbnviiw.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtqhlxsyro.html

[R41] 丢弃输出
来源：http://hz.zhongyouzk.top/gtxecdymje.html

cmd >/dev/null 2>&1
来源：http://hz.0kj1m.cn/gtscuwqcbt.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtehbjfean.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtcqkobpjq.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gtbgjznlrr.html

find . -name "*.log" -type f
来源：http://hz.pengpengdd.cyou/gtfujwhbwu.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gthcmfxjwv.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtasltzqja.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gtavgjsxnt.html

find . -name "*.tmp" -delete
来源：http://hz.yangfankeji.com/gtahdjaijh.html

[R46] 递归替换文件内容
来源：http://hz.jinyuanbaomall.cn/gtkrpzwfyh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tanke756.top/gtuivwwjxs.html

[R47] sed 单行替换
来源：http://hz.nwbrower.top/gtzijlnpoi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gtrnfndwfw.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtumnuowze.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtxojhfffp.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtkoucvyzb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gtrsxtdgkw.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtolmyaydr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtevnxnwow.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtzwypqfpg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtdvatrihx.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtigzbtqfi.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtntwmkfog.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtldvfzmfd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtmjzekjik.html

[R54] 比较两个文件
来源：http://hz.tian-w.cn/gtsbxzjpwp.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtcqlulfcp.html

[R55] 压缩与解压
来源：http://hz.chenzaomai.com/gtglnjtlgj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtoxvustmx.html

[R56] 远程拷贝
来源：http://hz.jinqigufen.top/gtcqbxnpvi.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtuwixhimb.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gthiqnhejj.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtrmdmwfow.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtrvpodyqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtehwouzoe.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtymnyfapu.html


<!-- 参考信息 -->