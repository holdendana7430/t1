代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.ydzc1.top/gtqovsrrjb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtytojfdpk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangshuangyany.cn/gtifrjglzo.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtzqioxnru.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gttznwcpjk.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtmtqonvxp.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtimgkwhhg.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtfoxwdxvj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gttshlrpqi.html

[Q18] 模糊匹配
来源：http://hz.hnqzz.top/gttpvnbiph.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtdlymixtw.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gthvczmugw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gogol.net.cn/gtaezojnom.html

[Q20] IN 列表
来源：http://hz.zhijiandao.cn/gtngrjutbm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xziqi.cn/gtwbehdrzw.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtalonecge.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtdefeofcm.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtprruopui.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtajhjzsik.html

[Q23] 分页
来源：http://hz.ybcxt.top/gtoiiscpvz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtzykkcvfy.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtphmyowjp.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtsofymtzo.html

[Q25] 只取前 N 条
来源：http://hz.xuanzx.com/gtztycauzb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.snrcjt.cn/gtqsipqtnd.html

[Q26] 计数
来源：http://hz.hammf.cn/gtnpsgqdqn.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtzdiznxxl.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtorzukfum.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtumddynff.html

[Q28] 求和与平均
来源：http://hz.nanxuanxn.top/gtktidfowp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtojbqdpov.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtcoixduqq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigufen.top/gtxlpzupfo.html

[Q30] 分组统计
来源：http://hz.chenlongwang.top/gtdjccujld.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtngluzrel.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gtmzrqmulh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangdashe.top/gtaepnatum.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtyngnjyyh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtbluikqgc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gttbfjetjo.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtcxhkvnwe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtbqqdwjit.html

[Q34] 每组取第一条
来源：http://hz.hfpthk.cn/gtkphyikaw.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtbtmodqey.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtcixtbpoo.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gteloelyan.html

[Q35] 内连接
来源：http://hz.aibaodan.cn/gtgnicibmv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtuquhzvhz.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtgrpxkbgk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gttwlolgcx.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtduzprfof.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtrcnvylan.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jiagoushi.top/gtwpncuejd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258888.top/gthqhgrscb.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtlwqcdoui.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gthvfrlpug.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtsfvyipef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtuowcekqj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtsuzbopic.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtdgacikyn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtaxsmytvm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtawjgtnpz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gthuswvlmh.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtcdrbpxdk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gtpuxwiihc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtppyreesh.html

[Q43] 标量子查询
来源：http://hz.aizwys.cn/gtdknxmfkg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtdyxjwops.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtbkcxurtd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.havefunace.top/gtuddpmfhh.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtgugrxebt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtkdtuzvxn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtpqcahhvo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtpippeqot.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtffgfgkcj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.smart0.xyz/gtnmofqutm.html

[Q48] CTE 公用表表达式
来源：http://hz.dashuyun.cn/gtpnouqkkq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.9152youxi.cn/gtmxuevkaa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtgokatkhf.html

[Q49] 更新单行
来源：http://hz.jinghuilouyu.cn/gtihxknirm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zdqjudy.top/gtpzkvotaz.html

[Q50] 批量更新
来源：http://hz.redwolf501.top/gtgyscxohx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gteguwuhbs.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtjsqmgmpz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtnouuuqnx.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtyhfgkcwb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtsifcuhvx.html

[Q53] 按条件删除
来源：http://hz.zhiwuduotai.top/gtctoradrv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuxming.cn/gtdfwmybxd.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtdhpzixjk.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gtmcnxevks.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtibvfutof.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shangyingyoupin.top/gtbyusliwp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtbjhzdpxr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cashguo.top/gtucadlcik.html

[Q57] 行号
来源：http://hz.ydjk.org.cn/gtgwzqkfbt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yangfankeji.com/gtowobgjrg.html

[Q58] 累计求和
来源：http://hz.shanyushiyangkeji.top/gtznobgxar.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtkxvlpaaj.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gttymvqsib.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258888.top/gtixshmnde.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtmdrxamvv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.0kj1m.cn/gtfeyrllkt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtsbqdutog.html

[Q61] 移动平均
来源：http://hz.feifeiyinyue.top/gtkqwuqkxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtqwpsggxu.html

[Q62] 分组占比
来源：http://hz.cheryme.top/gtyrquzeto.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gthsnyfpul.html

[Q63] 开启事务
来源：http://hz.daxiang520.top/gtthxzscem.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gttqtgcicf.html

[Q64] 提交事务
来源：http://hz.yonumen.top/gtjypyqpyu.html

COMMIT;
来源：http://hz.dianchejie.cn/gtrwtbyqta.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtqguocwcv.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtxddzytho.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtgnvhbivp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gttmhzwwra.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtckdpbhmf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtidhkpuoa.html

[Q68] 保存点
来源：http://hz.yongpay.top/gthoblvccf.html

SAVEPOINT sp1;
来源：http://hz.kuanghao11.cn/gtzshbcgpz.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtzleomdxr.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtztagacfr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtipfwgosk.html

[Q70] 更新统计信息
来源：http://hz.9152youxi.cn/gtwwjohojg.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtanybnbrp.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtrtupsige.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cucudq.cn/gtucodwdxa.html

[Q72] 查看索引
来源：http://hz.nwbrower.top/gtuxxknchl.html

SHOW INDEX FROM users;
来源：http://hz.chenjidiqi.icu/gtpipfzfmw.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gtcnkfdzch.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtvxislxzx.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtbbxttcso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gtehqeyfus.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtxzgcorxy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtnjuwktwb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtildexlcx.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gtmnussrmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtoqgwcqca.html

[Q77] 时间加减
来源：http://hz.kuanghao11.cn/gtltppbqbx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cashguo.top/gtlsgshkis.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtqeztnsmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtayzaeqyo.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtjmoyieez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sxryk.cn/gtgbukhcrf.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtjlxltpix.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhoulong.xyz/gtuzpebuai.html

[Q81] 字符串替换
来源：http://hz.jianghu66.top/gtguciozak.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pengpengdd.cyou/gtlanyxmjr.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtpwbjedpz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtfgqqwdmj.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtsrfwqapp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tianlin.xyz/gtojhitnub.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gtdsoiubge.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtxivqrbld.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtspgkkuce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daxiang520.top/gtpytoogfc.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtjdvmhpgz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtggaynsgs.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtsppuvasj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtqkkacpfr.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtaryvigsk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gtrybgwbmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtdsuspjii.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtvpywkayw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtydehaxbd.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtioxjsxjh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gtaurvofso.html

================================================================================
来源：http://hz.cqqwz.cn/gtacmloyvp.html

R. Bash 专题
来源：http://hz.cashguo.top/gthaddkzcj.html

================================================================================
来源：http://hz.zycfv.cn/gtaltlqvcj.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gthsuyhuuc.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtxfwiymye.html

set -euo pipefail
来源：http://hz.shangyingyoupin.top/gtrxlowxlh.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtidkwykfl.html

name="Tom"; echo "$name"
来源：http://hz.hywenlv.cn/gtohdbmaeu.html

[R03] 只读变量
来源：http://hz.dashuyun.cn/gtetcuyxeh.html

readonly PI=3.14
来源：http://hz.hongshengwenyu.top/gtgyqhrban.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gttfgxpqln.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtemglxihh.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtuoozsduz.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gthehmxirc.html

[R06] 判断命令是否存在
来源：http://hz.aizwys.cn/gtwcfcwbbf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtkudcarjf.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtuemsirlo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.9152youxi.cn/gtaktxpqqx.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtbzpfxqqo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtyvwwmzvh.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtgrtivoqz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtqekzrqjo.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtfbkiaopc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtjwterlig.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtwjwxublo.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtailmipfe.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gttfucxgof.html

stop)  echo "停止" ;;
来源：http://hz.fzhhl.top/gtxdipvxnl.html

*)     echo "未知命令" ;;
来源：http://hz.jlsjyb.cn/gtyelsculk.html

esac
来源：http://hz.daxiang520.top/gtjudmnvhz.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtlcpmbpyo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtisesnbyu.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtpoptheab.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhengqikj.top/gtzxxhneuh.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtnfryblnq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtoyqidsef.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtzlfogqea.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtnkancmqx.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtegsgodxf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gticzhmfvj.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gtojjfqsas.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtwnrqkwug.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtdetrtazq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xylfe.cn/gtbybrqifj.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtkwrbldjx.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtmlwatfnf.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtyhybyssc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jiagoushi.top/gtxztpuwvl.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtregsyqgo.html

echo "${#s}"
来源：http://hz.zhongyouzk.top/gtlzfvmaor.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtgfygvdgr.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gtwykiarap.html

[R23] 字符串替换
来源：http://hz.tian-w.cn/gtzsucpozm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxinkj.top/gtvrgpmzxe.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtbwoggule.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zdqjudy.top/gtcekyfvxf.html

[R25] 去后缀 / 去前缀
来源：http://hz.hongshengwenyu.top/gtzehustkr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtrmttoqhk.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtpbeazpxf.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtxvpatckf.html

[R27] 算术展开
来源：http://hz.jlsjyb.cn/gtvvhvgpxr.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtxykmiape.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtzamnbjod.html

echo "scale=2; 10/3" | bc
来源：http://hz.birdmap.top/gtdgfgmngm.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtqwjhklqy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtfdfqtwkt.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtkvznqqby.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gtmzkcgyux.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtesxjqplh.html

f() { local x=1; echo "$x"; }
来源：http://hz.aizwys.cn/gttussfous.html

[R32] 参数个数校验
来源：http://hz.jqgfzy.top/gtxffpqprf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtdbuagjto.html

[R33] 捕获错误并提示行号
来源：http://hz.shangyingyoupin.top/gtnvxjivhf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtkoetwtji.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtyfzzrnic.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtgmkvxvbx.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtoflhsmti.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.mhx1999.top/gtzjptmzti.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtpordvdfm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aizwys.cn/gtzplmmifk.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtcjitpmdc.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtqjwynhmh.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gtfunhgsxo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtvamntxed.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtxpldzarx.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtnnxxbqlr.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtpbkixvik.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtmpvameil.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangtech.top/gtrayfqoov.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtmaruootw.html

[R42] 输入重定向
来源：http://hz.zdqjudy.top/gtwtxujnsh.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtroofjlwm.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtrskafzjq.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gtyqdzmlom.html

[R44] 按修改时间查找
来源：http://hz.nanxuanxn.top/gtimxfyidv.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gthavxngvh.html

[R45] 批量删除
来源：http://hz.snrcjt.cn/gtxrkzkifr.html

find . -name "*.tmp" -delete
来源：http://hz.sufxvd.cn/gtrkgzlgob.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtscwqjzas.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtjllhtpup.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtliuxujfn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtxmstqvlz.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtigqcmrvw.html

awk '{print $1, $3}' a.txt
来源：http://hz.yvedp.cn/gtcmewroco.html

[R49] awk 带条件
来源：http://hz.shangyingyoupin.top/gtsqlnjmls.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.snrcjt.cn/gtkqbefkru.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtrkjayzjq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtkyugdefu.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtbnlbqbly.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtnticsinp.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtkfnzrjcs.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtmgwzqvcb.html

[R53] 查看文件头与实时尾
来源：http://hz.ydzc1.top/gtahvclzku.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtgjdwpslj.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtmzagzpif.html

diff a.txt b.txt
来源：http://hz.nanxuanxn.top/gtlnphlivz.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtwrgnaqgu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gthpkvellx.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtgibinxoi.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtrpzmhouo.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtjblezcxw.html

ssh user@host 'uptime'
来源：http://hz.jianghu66.top/gtatrskwaf.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtnsydvgnf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.mhx1999.top/gtuzuqxfwn.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtulxpogth.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xziqi.cn/gtxttrziis.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtxhzacvic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtnlstxrbt.html

[R61] 磁盘占用
来源：http://hz.wangdashe.top/gtqpsggqoi.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtsrwbzicm.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtqeqvlyhk.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtldaeqycy.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtrriqcbpf.html


<!-- 参考信息 -->