代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.quarkkingdee.top/gtlfzdyiyz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.9152youxi.cn/gtokimietl.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtipaakcmd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daxiang520.top/gtzuweoxij.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtvmtqdqxq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gtmvezieje.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtzoojqljj.html

[Q15] 查询全部
来源：http://hz.svipenyu.cn/gtvchueizb.html

SELECT * FROM users;
来源：http://hz.gotoacloud.top/gtlpsldnmy.html

[Q16] 查询指定列
来源：http://hz.tianlin.xyz/gtobumgjut.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtpdsylztm.html

[Q17] 条件查询
来源：http://hz.zhongyouzk.top/gtqwkrrera.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinyuanbaomall.cn/gtsaufporw.html

[Q18] 模糊匹配
来源：http://hz.feifeiyinyue.top/gtnqpbeptj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gteraztcpk.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtdxjnyshc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aizwys.cn/gthamrolhm.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtrrmxsqbj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtrleeatim.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtqhzdbgpm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtzenbbyvw.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gthkoebdzc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.bjfxy.top/gtjuukavrb.html

[Q23] 分页
来源：http://hz.bjfxy.top/gthwtvsnpj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tanke756.top/gtoosbcdmy.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtwvfqozfm.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtnleopoyw.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gthrbkfegf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gtraauddqy.html

[Q26] 计数
来源：http://hz.svipenyu.cn/gthwbucpja.html

SELECT COUNT(*) FROM users;
来源：http://hz.aizwys.cn/gtnxufegla.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtxberaynt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.birdmap.top/gtifafevmf.html

[Q28] 求和与平均
来源：http://hz.chenlongwang.top/gtvfhggtpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtvczjntmt.html

[Q29] 最大最小值
来源：http://hz.yongpay.top/gtrhquiils.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gthdtnrnvk.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtecnliyma.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtjitqomnv.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gtgmdjhpxs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtbfqwzznj.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtgnuxmixe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gthukjzumw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenlongwang.top/gtnjefcpyf.html

[Q33] 多列分组
来源：http://hz.gzhubu.top/gttidqwfpk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.smart0.xyz/gtjmbibpju.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gttqeefsxc.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtiunfygyv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtiqaugonl.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtauufybvh.html

[Q35] 内连接
来源：http://hz.pengpengdd.cyou/gtqxabfwem.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtgbasbeic.html

[Q36] 左连接
来源：http://hz.pycfn.com/gtqbfjlqwd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtbyjdypyt.html

[Q37] 右连接
来源：http://hz.yangfankeji.com/gtyzzklvrh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtrdfdemoj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gtkgkffeme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuetiantiany.cn/gtknbyqvyu.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtuestsyez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtfdsnolmo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gtbcrrzevx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhaomingkeji.xyz/gtyvqvmnux.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtelssvkgn.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtbznvmelp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtduhgwohr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtjuofhhjj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtmesoidur.html

[Q42] 连接条件附加过滤
来源：http://hz.sweek.top/gtnhrrcaos.html

SELECT u.name, o.amount FROM users u
来源：http://hz.316326.xyz/gtxhggoshj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtzfwtrsyp.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtugisyvpz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.birdmap.top/gtywkrnavy.html

[Q44] IN 子查询
来源：http://hz.gzhubu.top/gtsddprpde.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtlwkqkvlb.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gttkjblmbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gtfupayyaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xylfe.cn/gtxnbvdgyn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtcsbzezqh.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtxcpjxurz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtnfdlxzgr.html

[Q48] CTE 公用表表达式
来源：http://hz.gotoacloud.top/gtbdlegnug.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.vqdsnc.cn/gtrhqqiiqr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gtspdtgize.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtpddtzkos.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtvznvgdap.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gtxaefktkx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.redwolf501.top/gtmfjnpolx.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtihokrlwa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hywenlv.cn/gtghpkivxp.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gtddeyfosz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtabmcdhbn.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtjccvnxvs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtqycghkrm.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtobcnomoh.html

TRUNCATE TABLE logs;
来源：http://hz.dianchejie.cn/gtbueerfnr.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtjviwzlww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtwnxvwbpc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dashuyun.cn/gtohqapqqh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gotoacloud.top/gteacssnmg.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtplwuarla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gthxrmujgh.html

[Q58] 累计求和
来源：http://hz.shangyingyoupin.top/gtrnqdrxwt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtvltbcvli.html

[Q59] 分组内累计
来源：http://hz.nanxuanxn.top/gtskjpkgtq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtzfavyvms.html

[Q60] 取上一行 / 下一行
来源：http://hz.xingfuxueyuan.xyz/gtrljxwgll.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gtfmwkrflk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtvadesqyx.html

[Q61] 移动平均
来源：http://hz.hysaishi.cn/gtpvmhimzh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtygmmxiqa.html

[Q62] 分组占比
来源：http://hz.zhengqikj.top/gtuyulbewv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtkjnbshoe.html

[Q63] 开启事务
来源：http://hz.316326.xyz/gtituqjrnu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtpftlalma.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtvqdqdbus.html

COMMIT;
来源：http://hz.hammf.cn/gtmbuyrqni.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtcbiceato.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtjadmcpac.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtsnwklvel.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtvdbyxuwg.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtujymqqte.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guannengcc.top/gtfkxtayza.html

[Q68] 保存点
来源：http://hz.316326.xyz/gtueyapasf.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtxbwkahwu.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gthxhhzppn.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gteneazzvu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gtzucmgppa.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtqfvdqbyb.html

ANALYZE TABLE users;
来源：http://hz.cucudq.cn/gtisgnhtxl.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtgzgucrmx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinqigfzy.top/gtqteugqno.html

[Q72] 查看索引
来源：http://hz.kuanghao11.cn/gttuozxjer.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtrlrowxxc.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gtszzdwmge.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtcqobngsd.html

[Q74] 强制使用索引
来源：http://hz.nanxuanxn.top/gtvfrzmvby.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangdashe.top/gtircmtfjv.html

[Q75] 日期格式化
来源：http://hz.zycfv.cn/gtwmrgvsvl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtzzrzdakg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtqezjhmnn.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtgubayzpd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yanxiufei.cn/gtqavyrjyy.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gtbyarxhib.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gthoefwdcr.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtjqgndiie.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtdjnxrdda.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtuavwkmgy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtspecpdbl.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtiusaxdmc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtqeixmumi.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtcrnprqlv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtymexvaks.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtjcuhgicu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtpxxjxwbp.html

[Q83] 大小写转换
来源：http://hz.ydjk.org.cn/gtrkeqgnpr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtvrkejctl.html

[Q84] 去除首尾空格
来源：http://hz.svipenyu.cn/gtwtvigbse.html

SELECT TRIM(name) FROM users;
来源：http://hz.andypj.xyz/gtmjbnymlw.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtlybeiooh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtavubtejc.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtifmlmves.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtwfguejzv.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtzaellgft.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtnhznkqbg.html

[Q88] 行转列（条件聚合）
来源：http://hz.meibo888.top/gtvtmziryk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtcpalptll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gtjqeerkly.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtmjakqexc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtromokwir.html

[Q90] 生成序号列
来源：http://hz.bjfxy.top/gtzdengyps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gaohongyu789.top/gtkqiekgpp.html

================================================================================
来源：http://hz.havefunace.top/gtdtgcflhw.html

R. Bash 专题
来源：http://hz.cqqwz.cn/gtlcjikbfi.html

================================================================================
来源：http://hz.smart0.xyz/gthjjspwtb.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtyorczydm.html

#!/usr/bin/env bash
来源：http://hz.mhx1999.top/gtzmfneeke.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtwsxnegrm.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtqahzsils.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtlilkhdwc.html

[R03] 只读变量
来源：http://hz.zycfv.cn/gtnmsuxxhf.html

readonly PI=3.14
来源：http://hz.zhixingplan.top/gtjtglfiab.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtbsafkzqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtmejsagup.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtwcurgvcl.html

name="${1:-default}"
来源：http://hz.jiagoushi.top/gttaopjboy.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtiajbzebu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtrghwavca.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtxjimmkkq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtugycekxo.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtaemahjrb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtdteuhryy.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtbcpvydel.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtujybrnfb.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtmlysykvj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gttmlgezgp.html

[R11] case 多分支
来源：http://hz.gotoacloud.top/gtfeipftwt.html

case "$1" in
来源：http://hz.jianghu66.top/gtjlgneuoy.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gttkuocpao.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtpfbeantl.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtssxdpaip.html

esac
来源：http://hz.haohaochexian.top/gtiqlmiwcu.html

[R12] for 遍历文件
来源：http://hz.gotoacloud.top/gtftcpiqol.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gttudmpbkw.html

[R13] for 计数循环
来源：http://hz.jiagoushi.top/gtfmtrcjnf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtislvvjmp.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtuqrjdbwp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.c1oappe.top/gtuqtfayli.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtrvfzlzli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gttludgpom.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtwttqzqmg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtvuwglcse.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtybapiwqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gtigthlvpc.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtmiescdjr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pengpengdd.cyou/gtrulyesmr.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtwsuyokag.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtpqoqfmfe.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtjyypnvls.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gtglskdtcq.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtalqietmf.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtbkmflrns.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gttbmgiyry.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtuiiaifdf.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtvhwsyywp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtepdyhamx.html

[R24] 大小写转换
来源：http://hz.dianchejie.cn/gtsvpcxrib.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtpatentsw.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtdbjfebnh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhengqikj.top/gtvhxgmucs.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtlmpzoqnr.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtfrannkku.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtrtnxpvbv.html

echo $((1 + 2 * 3))
来源：http://hz.jiagoushi.top/gtfiadsgux.html

[R28] 浮点运算
来源：http://hz.fengsongda.top/gttzpzangr.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtgembrsxa.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gttdudpaqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.andypj.xyz/gtbhdbjezt.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtkuxayrxy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guannengcc.top/gtffflkyzy.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtwjekwfkh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gtrgrpqjdz.html

[R32] 参数个数校验
来源：http://hz.fengsongda.top/gtoutzyfiv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtryibisdf.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtncgaxjkt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtitzshhzd.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtoozzxhlz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtzvfriqar.html

[R35] 后台执行并等待
来源：http://hz.zhiwuduotai.top/gtjszbukad.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtypzmwxtc.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtkqdkbiso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gzhubu.top/gtjhnsqhch.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtggmgczqo.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtoraxofis.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtmduubkom.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yanxiufei.cn/gttcfzrvzc.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtqprjnpwv.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtrkppcnbl.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtpccrrmvn.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtaiawyadj.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtvyqlpgws.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtuftgswfa.html

[R42] 输入重定向
来源：http://hz.wangdashe.top/gtpeoctfvd.html

wc -l < a.txt
来源：http://hz.tianlin.xyz/gtdbofupnx.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gthgrxrkvx.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtsdozhbko.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtotkkpukc.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gtdnlmnkyn.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtivlxstrq.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtonmdoent.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gtgwuammpm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtkyzylkdf.html

[R47] sed 单行替换
来源：http://hz.jinqigfzy.top/gtgpodoisv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtjeleyjnp.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gtzgqxycqx.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtdfewmwho.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gthpihxkbb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gogol.net.cn/gtfgxlizyo.html

[R50] awk 求和
来源：http://hz.jinqigufen.top/gtixqsxtvu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhijiandao.cn/gtyingcxzp.html

[R51] 排序去重取前几
来源：http://hz.ybcxt.top/gthmsldvlo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gttboaovts.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtgiezavce.html

wc -l a.txt
来源：http://hz.c1oappe.top/gtpoqakmpw.html

[R53] 查看文件头与实时尾
来源：http://hz.chenzaomai.com/gtkegplwpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtrjwwqivn.html

[R54] 比较两个文件
来源：http://hz.hongshengwenyu.top/gtjnwrhmuv.html

diff a.txt b.txt
来源：http://hz.chenzaomai.com/gtvcypzhiu.html

[R55] 压缩与解压
来源：http://hz.316326.xyz/gteeyimmis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtafvjmgmc.html

[R56] 远程拷贝
来源：http://hz.sysykeji.top/gtwjpmrrvo.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtnsqjtpfj.html

[R57] 远程执行命令
来源：http://hz.pengpengdd.cyou/gtjsgwszlp.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtkkljrybk.html

[R58] 下载文件
来源：http://hz.nanxinkj.top/gtldbyzxiz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtsninybko.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtxmzyekdt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tanke756.top/gtcfoenwki.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtrufuhcft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gttdahdvuq.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gtxrkrgpht.html


<!-- 参考信息 -->