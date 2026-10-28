代发 wailian999

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtserbbbek.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtejyptrnl.html

SELECT id, name FROM users;
来源：http://hz.vqdsnc.cn/gtrftlzyxm.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtgvschnpj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtxisrblyi.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtlcbijyuh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pycfn.com/gtigojuvht.html

[Q19] 范围查询
来源：http://hz.xylfe.cn/gtiiugggzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtkjrfivov.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtjjuhgorv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtrqtrofdy.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gtwqbmzrlj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.haohaochexian.top/gtztwollyf.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtaxbzoxvm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtxclcquvg.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtrgsqhwst.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtiojhuyla.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtcrlqgsoq.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtvoiesabt.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtdcvrimid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtudwgjqff.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtbyjlclek.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtfswrcymt.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gteqrktfxs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtgofuhcpy.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtrcqjqnvt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtrlhzrhve.html

[Q29] 最大最小值
来源：http://hz.sxryk.cn/gthmpygvhs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhengqikj.top/gtxxxrcflv.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtxqerzrjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtydndfmij.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtnnymqclw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtwiwglwjj.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gthjgbvoxj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gthpeqnsbk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtilzdgqkn.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gtqrzuicah.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangshuangyany.cn/gtzfzpzkbr.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtliiymjcf.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gthfbpfoti.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fzhhl.top/gtbvrkhrev.html

) t WHERE rn = 1;
来源：http://hz.jianghu66.top/gtznqmcwbz.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gtozppgugs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gthglwhpku.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtskylohdn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtriydtxoy.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtoetbklqp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtlyrcnevv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtxllnpzvc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aibaodan.cn/gtlrrlsofa.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtmtmlksue.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtwqomfcyy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.haohaochexian.top/gtuprfurzb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtquvuorjz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtdfdinqgj.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtypzopiut.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gteszeqvbh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtyqgfwfgi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtgditengd.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangkeji.top/gtwucrgocj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gtveneqxcl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jianghu66.top/gtxupsbcyu.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtqosjwptu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtusclslcc.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtblgaiuwu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nwbrower.top/gtlccawgkn.html

[Q45] EXISTS 判断存在
来源：http://hz.jianghu66.top/gtewlceaav.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gttfrrtugr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtxtgoeoac.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtutijfjjn.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtfhtgobid.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gturifcrcr.html

[Q48] CTE 公用表表达式
来源：http://hz.yueranfly.top/gtmarlhwpq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtwcsjftpn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.feifeiyinyue.top/gtrfrypefx.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtsihnkvjw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtfzaepagr.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtkbealooo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtldcnavuo.html

[Q51] 用子查询更新
来源：http://hz.dashuyun.cn/gtoobtogkq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtibvkgdma.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtcfkcfaca.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gtvxxqazvs.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gtxkfeesxe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtuwvluowy.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtvjkvsard.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtluexdkuq.html

[Q55] 排名（并列占位）
来源：http://hz.dianchejie.cn/gtdbovepof.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxuanxn.top/gtondhunoe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.redwolf501.top/gtsjtjnjxo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtjskhpgrg.html

[Q57] 行号
来源：http://hz.jinyuanbaomall.cn/gterevtjew.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangdashe.top/gtwektolvv.html

[Q58] 累计求和
来源：http://hz.chenjidiqi.icu/gtfhjdxbbw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gtpiiohiki.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtxrvjvjtn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gtpjxqgwfc.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtbnglkqyu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtkbfgxgdl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtatckwgsq.html

[Q61] 移动平均
来源：http://hz.chenjidiqi.icu/gtchchsozb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gttznrlidp.html

[Q62] 分组占比
来源：http://hz.daxiang520.top/gtqeosgznc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtxllrgpdy.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gtiudpxqqx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.mhx1999.top/gtqqemcgdh.html

[Q64] 提交事务
来源：http://hz.snrcjt.cn/gtiivboafv.html

COMMIT;
来源：http://hz.sysykeji.top/gtdhaxowcf.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtdmzpvqaw.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtthwvuybx.html

[Q66] 行锁查询
来源：http://hz.yvedp.cn/gtouxdldwd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtcrzgwebq.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtalnkknah.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gttbahgzsq.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtqornhzxh.html

SAVEPOINT sp1;
来源：http://hz.zycfv.cn/gtyfoesqpi.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtxrhvrrbr.html

[Q69] 查看执行计划
来源：http://hz.jlsjyb.cn/gtyeciival.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtqylsibvf.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtowapxriq.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gthxzqcutk.html

[Q71] 查看建表语句
来源：http://hz.svipenyu.cn/gtnhzafywh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.vqdsnc.cn/gttprlmstr.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gtpcgyrwim.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtjjlkmgqu.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gtmkrkrsin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtjlktjowl.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangkeji.top/gtazhsgmsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtkdlhumpy.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtxcauhwet.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtenefpbdp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenlongwang.top/gtpsknfrbs.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtpplmuuhy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtlrvqqpcc.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtwmnwlrcn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhongyouzk.top/gtfegznrpp.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gttbbqutev.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydjk.org.cn/gtwavcwkbm.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gttegbpjni.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtlqwkwjut.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtaqnkmnfv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtmdeeidrw.html

[Q81] 字符串替换
来源：http://hz.gotoacloud.top/gtbbklxjbe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtusiepszj.html

[Q82] 字符长度与字节长度
来源：http://hz.xingfuxueyuan.xyz/gtaennqntg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.redwolf501.top/gtvcdebbsz.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gtqurlbsuj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtvdpvtrge.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtrleccfjx.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhoulong.xyz/gtjaewxwho.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtfjjvmusv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtxaomkbqd.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtafmbdynv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtltyeoyld.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtqzghjfwd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gttauzexyh.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtyhxzvqpj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj20258888.top/gtfueauatq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtqcxqomub.html

[Q89] 判断表是否存在
来源：http://hz.pycfn.com/gtwgjemfmi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gttjgsmtne.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gtefkoumjh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yongpay.top/gtpzauxxby.html

================================================================================
来源：http://hz.ppjwa.cn/gtvsedthuv.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtjkpryghd.html

================================================================================
来源：http://hz.gzhubu.top/gtfrgpcxfs.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtwcxiqtrv.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtagxoqnks.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtseiihnyk.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtankdxiox.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtkihknzuf.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtgyizevby.html

readonly PI=3.14
来源：http://hz.gaohongyu789.top/gttglinfef.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtulwnurkn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hongshengwenyu.top/gtitombkfn.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtnlcoftqy.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gteuqifhbx.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gtfusetixa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydzc1.top/gtancaarjd.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtbkjsvrik.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtrkfoaaax.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtxeueglew.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtusgrzmtl.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtuhlkjnzo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtcudgqvyi.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtxgmpwzlc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtnfywoauk.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtgnezhxoz.html

case "$1" in
来源：http://hz.zhixingplan.top/gtobeybmjz.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtneleuqnw.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtessvzsqz.html

*)     echo "未知命令" ;;
来源：http://hz.tanke756.top/gtwlifmemt.html

esac
来源：http://hz.ivvv.top/gtfxvubiiw.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtsageljhr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gthzplotwa.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gtsopogjxw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtrwijdosp.html

[R14] C 风格 for
来源：http://hz.yj20258.top/gtijjepurb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtfzkdhdlb.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtbgppltub.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtzhuzdeph.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gthmzwjfcf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtqmgmbwnq.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtbxuspiff.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtocughmqb.html

[R18] 遍历数组
来源：http://hz.redwolf501.top/gttmyfvzyz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gtixlrzghd.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtwzhjnjnf.html

echo "${#arr[@]}"
来源：http://hz.dashuyun.cn/gtgprxfxlw.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtmlvrmgdf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jianghu66.top/gtlglcpxkb.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtucuabbtm.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtaujsuzxr.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gttcvimlhh.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtxwinxuxb.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtxhvhljhr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yvedp.cn/gtdcycdsgf.html

[R24] 大小写转换
来源：http://hz.sysykeji.top/gtmdncwkud.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuetiantiany.cn/gtwfcecjba.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtbzmdjllz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtotidqoug.html

[R26] 命令替换
来源：http://hz.xziqi.cn/gtaurybomx.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtybjwraxj.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gtecitznlp.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtvuwapnmz.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtxrmrmrcu.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtsodxlnur.html

[R29] 定义函数
来源：http://hz.zdqjudy.top/gthbrfhhon.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtfvljxbpf.html

[R30] 函数返回状态码
来源：http://hz.iojbl.cn/gtnmvznord.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtkmuobsbe.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtipupritg.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtpymxepfc.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtxzryreyi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtvnkwlmjh.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtsydjmycx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gtunvbscwx.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtbzdztxln.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtyqavfwxf.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtuesogsfi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gtnwwjqlus.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gtptpldtiz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydzc1.top/gthbskyshd.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtphaqhcye.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtnmjccyua.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gtxnwqnskt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtgusckbiv.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtxsudhpvh.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtgnovvsyp.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtscaibxvc.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtkesfkgbc.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gtuijvujpe.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gtaleaxniw.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtlfjdeddg.html

wc -l < a.txt
来源：http://hz.jyoumei.cn/gtebswbpdd.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtufradiby.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtvabtzwvp.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gtzhwetcxh.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtyklrxbkm.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtlhcrbxpw.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtfpybpaau.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtrcnpfdxw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xingfuxueyuan.xyz/gtplrdmutz.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtvmkmjylx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhixingplan.top/gtdjhxcitn.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtinkuinoi.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtgguvcasm.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtilsjjhhe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtrftdktof.html

[R50] awk 求和
来源：http://hz.hammf.cn/gtccjqzhcf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.0kj1m.cn/gthxitcaka.html

[R51] 排序去重取前几
来源：http://hz.ydjk.org.cn/gtnhwzgyuz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gtviwamqhh.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtkbmgkcms.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtrpznxffu.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtqlpwkdtg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtglnztdoo.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gtyopwydkd.html

diff a.txt b.txt
来源：http://hz.jianghu66.top/gtfvpmywbd.html

[R55] 压缩与解压
来源：http://hz.hongshengwenyu.top/gthxtishim.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangkeji.top/gthctexqfh.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtywykvgph.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtuvtxicuo.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtqpqkxchi.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtticgmxqc.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtwmhgrdib.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hywenlv.cn/gtuevhewqp.html

[R59] 发 POST JSON
来源：http://hz.dashuyun.cn/gtfzyznawv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gttggujlog.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gttufvyrsc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtcuxndmrg.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtpbubtjer.html

df -h;  du -sh *
来源：http://hz.yj20258888.top/gtfktpmhha.html

[R62] 找最占空间的文件
来源：http://hz.feifeiyinyue.top/gtlyhwgfth.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gttriekvmc.html

[R63] 内存与进程
来源：http://hz.316326.xyz/gtuamyzutq.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtsvfmycdx.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gteicujiyc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtlydgvzxz.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtemyusqtw.html


<!-- 参考信息 -->