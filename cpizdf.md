代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shuidangran.top/gtczbjlapm.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtjibyajsz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtjusqfqea.html

[Q10] 插入单行
来源：http://hz.tianlin.xyz/gtxfvydwcb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gtzdhlnwzt.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtyajdsfjr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhoulong.xyz/gtcxsdyrfa.html

[Q12] 插入后取自增 ID
来源：http://hz.hywenlv.cn/gtykzaegni.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.smart0.xyz/gtzhyqvpzr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gtvgpkvqnc.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtpjrlxvvl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtnhvtjfjr.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtdrtftqif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtjvvszwsd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtleivurrj.html

[Q15] 查询全部
来源：http://hz.mhx1999.top/gtggpdypno.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gthmyjlnnr.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtewuzwqqq.html

SELECT id, name FROM users;
来源：http://hz.havefunace.top/gtlsqvlcks.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtzivaphay.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtufayvtgw.html

[Q18] 模糊匹配
来源：http://hz.jinyuanbaomall.cn/gtssvbmfnx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtgrimjwci.html

[Q19] 范围查询
来源：http://hz.cheryme.top/gtxxlgjiwe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gtspgrrdxp.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtjczyehbu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gthodrxyod.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtvcvsoyex.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxinkj.top/gtkjtazscq.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtwbvvmgtr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtrkfdqctm.html

[Q23] 分页
来源：http://hz.ydzc1.top/gtshzcxaqt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gteknshvif.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtlyfcgknh.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtnidlxcua.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtbqmetnki.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtrrotrjvk.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtmelpmvkk.html

SELECT COUNT(*) FROM users;
来源：http://hz.dashuyun.cn/gtyirefrru.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtbjtntycl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.smart0.xyz/gtzhmtekol.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gttpoayclb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtgfwqzpkw.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtrmubtcrm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtalkyqubf.html

[Q30] 分组统计
来源：http://hz.yj202588.top/gthprgcrfq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtmvxtdblr.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtwzqqhnfz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtjbfiulpk.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gtmprwcyet.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtfaisuewh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gtbrqbczdr.html

[Q33] 多列分组
来源：http://hz.gaohongyu789.top/gtrrpsvvnc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xylfe.cn/gtcsimdfms.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtszyajfnj.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gtxydxeqvs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hysaishi.cn/gtuniymbpq.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtymerurmc.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtmsaxwcnc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtkzelamox.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtahmhnfhl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gthtgrdtex.html

[Q37] 右连接
来源：http://hz.birdmap.top/gthstsdngj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtnyrzfzmf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gttdjzwbbv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gttjjxpnmz.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtvmdkccqg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtieksbijv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtoimrdqzz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtrtvzdnzd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gtesyjgktq.html

[Q41] 多表连接
来源：http://hz.jyoumei.cn/gtislghbby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangshuangyany.cn/gteidjkpii.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtortfimow.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.52xcode.cn/gtigpfzmht.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gtuosbcnto.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cucudq.cn/gtpxablhfk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ivvv.top/gtuwtazxqy.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gttlotuixe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtcaaiulmu.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtyfdshxsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gthnhhbkqc.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtonkczrzb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtfiperkzf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtdqmhcnaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtzaeopcfg.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtuhoiobuw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hammf.cn/gtpzrwbxhw.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtijcoswve.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sxryk.cn/gtmmgtjcni.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gthlffgbic.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtuvzhinka.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtbfraveja.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gttvlsiuli.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtwtswsckt.html

[Q51] 用子查询更新
来源：http://hz.xylfe.cn/gtfiqqfrae.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gogol.net.cn/gtpfcmiqmf.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gtvxfowjwy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gtkqrahkgt.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtovnvffne.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtcraxyuvr.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtghxwsuza.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtroznmjof.html

[Q55] 排名（并列占位）
来源：http://hz.havefunace.top/gtemtmtnab.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gtjyvghkxh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtteuolphb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.316326.xyz/gttgwbwljt.html

[Q57] 行号
来源：http://hz.meibo888.top/gtspfdjzxo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gtmxtufjnb.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gtjjhghkys.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sweek.top/gtalhykonc.html

[Q59] 分组内累计
来源：http://hz.pycfn.com/gtsijigfvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtkmmdtmsa.html

[Q60] 取上一行 / 下一行
来源：http://hz.haohaochexian.top/gtlxeguvli.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtnoenremc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtqgtxhhdy.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtrwoyobge.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtqohcagbr.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtjblnvcdt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtelunrydd.html

[Q63] 开启事务
来源：http://hz.jinqigufen.top/gtbwxccvgo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guannengcc.top/gtkvyvxhlv.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gtosgnzjnb.html

COMMIT;
来源：http://hz.nwbrower.top/gtpsyuvali.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtrpkxvhud.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtafigingc.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtguahlpxs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtfnmtnjza.html

[Q67] 设置隔离级别
来源：http://hz.hfpthk.cn/gtlxyvobct.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cheryme.top/gtocevnelk.html

[Q68] 保存点
来源：http://hz.smart0.xyz/gtvhvorbdu.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtmtjdaqon.html

ROLLBACK TO sp1;
来源：http://hz.hywenlv.cn/gtoyhtnabe.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gtqyatrotr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtoemuemxj.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtphioooxi.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtqqzxxbqk.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtecarnwgb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gtekxiicbx.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtwtdpojax.html

SHOW INDEX FROM users;
来源：http://hz.wangshuangyany.cn/gtbddxivet.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtmruhuxkr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtchogwcog.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtsxwfzbue.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtfoljxnox.html

[Q75] 日期格式化
来源：http://hz.sxryk.cn/gtdeoyytan.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxinkj.top/gtaiawaprf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.52xcode.cn/gtoohkrmvn.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtijikepkk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtdjlzlfar.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gteddfkrlq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtvbwegubb.html

[Q78] 当前时间
来源：http://hz.jqgufenzy.top/gtafwzuvub.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtywmvpsvl.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtcmmvlybd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtlxwskmfu.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gtshweaszk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnxiangtu.top/gtmslipbci.html

[Q81] 字符串替换
来源：http://hz.cqqwz.cn/gttmntvnwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtgupyijum.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtrbanxmsj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.iojbl.cn/gtvwfdybsg.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtbtctjkxv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtoimffcsp.html

[Q84] 去除首尾空格
来源：http://hz.guannengcc.top/gttmyagomu.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtmjlljwnh.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtzmlyawec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtxcrsswwn.html

[Q86] 读取 JSON 字段
来源：http://hz.mhx1999.top/gtkdjpewbr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gttmyanyar.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gttahvhgsy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gtqygvcfrn.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gtbgmzcxpa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgufenzy.top/gtubgnjwke.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtznxixdwg.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtqqjgjcyj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gtfsuxmwtu.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtjjarswxw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtsbhgccjs.html

================================================================================
来源：http://hz.aizwys.cn/gtomedrczm.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtsmosprqz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxtrcxlay.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtzyhwcgtj.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtvhopttxf.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtfiklwhqn.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gtzzmxatjg.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtznrnknmb.html

[R03] 只读变量
来源：http://hz.ivvv.top/gttjadsshc.html

readonly PI=3.14
来源：http://hz.feifeiyinyue.top/gticxrznqp.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gttybojhor.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tian-w.cn/gtjqiuaudh.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gtenkluktj.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtqxdttelz.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtrluibrdb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtpuqjxnkr.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gttayyznkk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtkpdyscxm.html

[R08] 数值比较
来源：http://hz.tianlin.xyz/gtcwtziszg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtuafwpchv.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtusoteofg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gtjlljjqai.html

[R10] 正则匹配
来源：http://hz.zhengqikj.top/gtouongpoj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtvmhlwvas.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtetlkkwuj.html

case "$1" in
来源：http://hz.birdmap.top/gtbjcvoaip.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtmbrurfix.html

stop)  echo "停止" ;;
来源：http://hz.redwolf501.top/gtufnwziwz.html

*)     echo "未知命令" ;;
来源：http://hz.jqgufenzy.top/gttrhpxceb.html

esac
来源：http://hz.haohaochexian.top/gtquznlzkw.html

[R12] for 遍历文件
来源：http://hz.xziqi.cn/gtmctmtktr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gthgijrugv.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtnkxajpjg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtejhcqygi.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtlknppeeg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gtbbjocuxm.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtuoghwrar.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gttiakryfq.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtgjmtjnwl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtqdopnfgm.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtqwjsxqxw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtolitcmek.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtbynssird.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtiagvfcov.html

[R19] 数组长度
来源：http://hz.yangfankeji.com/gtghudcsfl.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtaeggyqaw.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gthbrxqfuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtidsylvbu.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gtmdbrgacr.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtecyxtilq.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtpvvksttc.html

echo "${s:0:5}"
来源：http://hz.hfpthk.cn/gtrjrpfheq.html

[R23] 字符串替换
来源：http://hz.wangdashe.top/gtvsrvzgzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtntkvssxq.html

[R24] 大小写转换
来源：http://hz.iojbl.cn/gtwlpizxqw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtyjmfewns.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtdazsxaxk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gaohongyu789.top/gtulpjaafc.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtfkqpbieb.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gtelwwyvjw.html

[R27] 算术展开
来源：http://hz.daxiang520.top/gtaafbpmep.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtbztsfvss.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gtrxnnhbak.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtjhxjydrm.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtnvlvmryc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuxming.cn/gttetuejie.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtlzhjnnwg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtkdeexuca.html

[R31] 局部变量
来源：http://hz.ywan-chungtsiang.top/gtnbqtzhbv.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtwenfztzu.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtywrkitig.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtlzceveem.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtkxeuyaxk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtqqdsoilw.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtwzzwfpbc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtzoprfdjk.html

[R35] 后台执行并等待
来源：http://hz.zhoulong.xyz/gtyodhugxw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ivvv.top/gtubazfhlk.html

[R36] 并发执行多个任务
来源：http://hz.yj20258888.top/gtyewlmxir.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuanzhike.top/gtwatzcbur.html

[R37] 把输出赋给变量
来源：http://hz.cdnleiting.top/gtglfccgfh.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gtqcamlwlh.html

[R38] 管道串联
来源：http://hz.guannengcc.top/gttlwodgpi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangtech.top/gtoabbhrir.html

[R39] 重定向标准输出与错误
来源：http://hz.sufxvd.cn/gtfdzlashv.html

cmd > out.log 2>&1
来源：http://hz.zhiwuduotai.top/gtejtmyfpb.html

[R40] 追加写日志
来源：http://hz.chenlongwang.top/gtgapxahvj.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtpgejycct.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gtglnconrb.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtsvalgkkb.html

[R42] 输入重定向
来源：http://hz.ppjwa.cn/gtwfvxqklo.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gttnkuhpif.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gtaxqlqwtc.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gtyxyynsne.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtarledtxu.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtqlyhjabt.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtxnzmdyrh.html

find . -name "*.tmp" -delete
来源：http://hz.tianlin.xyz/gtcmcijheu.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtqecgclnm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtlrjvgtoh.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtrkdfxmpz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gttbjfwabs.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtggrqasxb.html

awk '{print $1, $3}' a.txt
来源：http://hz.hfpthk.cn/gtydrcgyba.html

[R49] awk 带条件
来源：http://hz.quarkkingdee.top/gtbdedqkha.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtrvyuncdv.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gtduycleqg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258.top/gtpnsockrr.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtoiuecobb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtowozziud.html

[R52] 统计行数
来源：http://hz.pycfn.com/gtimjkjipx.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtbesrfepq.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtnexrecwr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtrdhjrspr.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gtqppzpwie.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gtxwjopwye.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtvnfdfbxn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtpptlkzxe.html

[R56] 远程拷贝
来源：http://hz.yonumen.top/gtfqjcbkto.html

scp file user@host:/path/
来源：http://hz.jinghuilouyu.cn/gtdaumilhg.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtuqvkcqdy.html


<!-- 参考信息 -->