代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shangyingyoupin.top/gtltrmlnjh.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtwzzchbjz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pengpengdd.cyou/gtlpitywcn.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtjuyjjulf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtvpvwgozo.html

[Q24] 去重
来源：http://hz.ehwqpu.com/gtqpgbndxm.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtnuzjunay.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtpisyoxnj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jyoumei.cn/gtykvgyepg.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtoexjxohd.html

SELECT COUNT(*) FROM users;
来源：http://hz.smart0.xyz/gthehojisu.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtfbgyzbdp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gteowhlwfk.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtfnqqqvlv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtdrrsevhl.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtvazjwaxp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtjnoitchs.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gttnowhsju.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtmnyaucsi.html

[Q31] 分组后过滤
来源：http://hz.pycfn.com/gthmyznlzi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.svipenyu.cn/gtlxwnnfyw.html

[Q32] 分组拼接字符串
来源：http://hz.yangfankeji.com/gtnczwtylk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtktbeicxb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ehwqpu.com/gtbvatbbap.html

[Q33] 多列分组
来源：http://hz.chenlongwang.top/gtgpgpblwk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtyxcivqhe.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtvrxvpwox.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtmyecpsut.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtmrlifmrv.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtnosdyasi.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtpajszwbc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtpujefdtm.html

[Q36] 左连接
来源：http://hz.redwolf501.top/gtzloprflw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtrqxysutg.html

[Q37] 右连接
来源：http://hz.gzhubu.top/gtriptxtqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydjk.org.cn/gtiwobxons.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtpfvrcqdv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cdnleiting.top/gtqaxqfznr.html

[Q39] 自连接（查上下级）
来源：http://hz.zdqjudy.top/gtzohnyomw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtkpednkkf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtnulwgjug.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtgiqpbtmo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.birdmap.top/gtsytrdnvl.html

[Q41] 多表连接
来源：http://hz.yvedp.cn/gtuaiufovb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.iojbl.cn/gtjbupghda.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtmuhwxubb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigufen.top/gtkaqzumtx.html

[Q42] 连接条件附加过滤
来源：http://hz.havefunace.top/gthjpgvjfm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtpsouhqye.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.feifeiyinyue.top/gtcfucywvy.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtfgrvioas.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtzcaqepte.html

[Q44] IN 子查询
来源：http://hz.jinghuilouyu.cn/gtxrdpocvb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtymmkgsdw.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtgbtmukdj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtxsaphdwx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.feifeiyinyue.top/gtwsduskdx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtqcycpmgd.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gtmufgkxsg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj202588.top/gtjqlelupw.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtcopwduvs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtwcdrfljj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.0kj1m.cn/gtughdnate.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gthvrwqvgt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daria6918.cn/gttaeuyzxk.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtehbpppaq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtgdtkvbyv.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtmgubadyb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtklhuyttf.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gthdueqzsb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtvwiffgmn.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtfnhysugx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtjteyfdmb.html

[Q54] 清空表
来源：http://hz.guowangkeji.top/gtbfszmrzi.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtlkuxnenx.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtbcxkmycn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gtlebowhay.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daxiang520.top/gthdrtasua.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtlhowvdhe.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtninnizdo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtyzzsjigw.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtbwhxtytk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258888.top/gtojknpbay.html

[Q59] 分组内累计
来源：http://hz.gotoacloud.top/gtexalkbwb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtmefyixjj.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtkjqrkkbm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtffkzbruh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pengpengdd.cyou/gtueakfpmk.html

[Q61] 移动平均
来源：http://hz.zhijiandao.cn/gttbkhfhhv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.feifeiyinyue.top/gtagkptgfh.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtgavclwva.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gturspkgsz.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtuphqjmue.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ppjwa.cn/gtwyorthuq.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtjjwxbhkl.html

COMMIT;
来源：http://hz.xuanzx.com/gtnjlcyjly.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtdwzwafhd.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtrhxqhbod.html

[Q66] 行锁查询
来源：http://hz.tanke756.top/gtunqfqqvb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtwzsmoytr.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtklmkgtad.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gtjuqkukbb.html

[Q68] 保存点
来源：http://hz.birdmap.top/gtufwatfyj.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtrjvrwfre.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtbfuyggld.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtotyewtji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtohpxflja.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtcinkrqpq.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtdnwyqffw.html

[Q71] 查看建表语句
来源：http://hz.jinghuilouyu.cn/gtzukgguyu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhixingplan.top/gtjznuhxvq.html

[Q72] 查看索引
来源：http://hz.sxryk.cn/gtbfkivfjd.html

SHOW INDEX FROM users;
来源：http://hz.gzhubu.top/gtrikkqoqv.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtxhdhgxen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtivvceelw.html

[Q74] 强制使用索引
来源：http://hz.sxryk.cn/gtatodfyzw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtrnkdicmw.html

[Q75] 日期格式化
来源：http://hz.wangdashe.top/gtxjqkzrgp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtimaaszil.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtjqrwosgs.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtmuxuicco.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cqqwz.cn/gtheinixbz.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtlkjbzgii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtpjidleyr.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtldypxlfq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtsigrewyk.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtjlqzhmht.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.mhx1999.top/gtakunteyz.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtaevphmiw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tianlin.xyz/gtzzswwsob.html

[Q81] 字符串替换
来源：http://hz.havefunace.top/gtqpinbopp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gtcwabmumk.html

[Q82] 字符长度与字节长度
来源：http://hz.chenjidiqi.icu/gtfnrwrpxn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jyoumei.cn/gtdjasogbf.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtjxdtxzxe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtmldlkieu.html

[Q84] 去除首尾空格
来源：http://hz.jinqigfzy.top/gtommkshej.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtjfiwpier.html

[Q85] 数值取整
来源：http://hz.hammf.cn/gtinfalzol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtgvufzbes.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtvdsmfyra.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtrshbffpv.html

[Q87] JSON 字段做条件
来源：http://hz.zhiwuduotai.top/gthgmsbbyg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtuirmxxnx.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtaiqszzrp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtyjcldfhy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhiwuduotai.top/gteluckwjx.html

[Q89] 判断表是否存在
来源：http://hz.yvedp.cn/gtkpictruc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtqmygbfxs.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtaahbmfsz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gtsitenwku.html

================================================================================
来源：http://hz.daria6918.cn/gtuslxymfn.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gtuwjeldnn.html

================================================================================
来源：http://hz.yonumen.top/gtzubmwemq.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtmqjwuwhs.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtalhfzlyb.html

set -euo pipefail
来源：http://hz.gogol.net.cn/gtazpgxqrv.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtmlifqncc.html

name="Tom"; echo "$name"
来源：http://hz.haohaochexian.top/gtohknpram.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtpkmjqbpm.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtqplxsyxl.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtwjuqqqpz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tianlin.xyz/gtwkanpvjz.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtpjrypdcg.html

name="${1:-default}"
来源：http://hz.chenzaomai.com/gtlqnmqkuf.html

[R06] 判断命令是否存在
来源：http://hz.shzxlz.cn/gtbxcodeys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtticjtpvv.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtsjolwzwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtfwnxfjcv.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gtaoujbjrn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtcgybnvqb.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtnrvfoyzu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtwlgesszn.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtbrnoeghw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hfpthk.cn/gtlfotlqac.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtjpqwwtrf.html

case "$1" in
来源：http://hz.meibo888.top/gtpstlhxaq.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtfbetiiwk.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtvdhiadwe.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtgrkxhjms.html

esac
来源：http://hz.jinghuilouyu.cn/gtrmkayfsc.html

[R12] for 遍历文件
来源：http://hz.hfpthk.cn/gtlqbchhya.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xinyue.icu/gtdewwdvxt.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtsbfklnwu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sweek.top/gtuasduqku.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gtjbazyowk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuxming.cn/gtvykrmpws.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gtsnbmzjga.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.smart0.xyz/gtwntjmgqg.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtvtyghsqj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtwhgksqze.html

[R17] 数组定义与取值
来源：http://hz.guowangkeji.top/gtxmviltls.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtxqirjmue.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gtvcjfiyaq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtwibkkjhp.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtdhyacpsg.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gthfjmkcaj.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtwrnehefk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtvqodgxxo.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtdpbihqld.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtogwrodda.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtxndkmmgd.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtrmzbfpyu.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtjorkbhek.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtpivxczyk.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtghcciewi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtfzabfwky.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtyxfwdysl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtjzereeky.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtqliwnfqh.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtzezsdvzl.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtnkzydpch.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtdevgibcs.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtxhwiqywr.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtcadsepfq.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtfgsxwolk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gttmrhmhfn.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtpipkbnpr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtmxlewscw.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtezqgyhgx.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gthacqzfoc.html

[R32] 参数个数校验
来源：http://hz.jlsjyb.cn/gtldzasusm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gthpqeruho.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtqbkqagzk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hfpthk.cn/gtgxonoebc.html

[R34] 退出时清理
来源：http://hz.mhx1999.top/gtthyhcevh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtpoiuzpmr.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtknyyowmt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.9152youxi.cn/gthwmjmqrs.html

[R36] 并发执行多个任务
来源：http://hz.meibo888.top/gtxzrkuojf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.svipenyu.cn/gtxxleofie.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtzazbiick.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtwvrguesu.html

[R38] 管道串联
来源：http://hz.tanke756.top/gteuzbezdj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hammf.cn/gtolkklgip.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtymbdiosc.html

cmd > out.log 2>&1
来源：http://hz.dianchejie.cn/gtnszmwwlu.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtcmdtffws.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtotrpaqxx.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtvygtmoho.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtztuqcxxj.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtrqwyqyau.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtiwbnrscg.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtttldbxvz.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gthighoxkj.html

[R44] 按修改时间查找
来源：http://hz.vqdsnc.cn/gtlijifdrm.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtwmlldubp.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtlyyphvlf.html

find . -name "*.tmp" -delete
来源：http://hz.tianlin.xyz/gtljcabjsg.html

[R46] 递归替换文件内容
来源：http://hz.yvedp.cn/gtpoktmwsi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtgswghwbd.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtjziefyud.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtkynudeya.html

[R48] awk 取指定列
来源：http://hz.svipenyu.cn/gtknwgryol.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtknnrloft.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtaoycopkn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtzpcxkyzw.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtudqfajqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtdampgazr.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtufhzhrbt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtrisowipz.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gthphrpfob.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtdamqvsyh.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtgtabrsek.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtzxzektjl.html

[R54] 比较两个文件
来源：http://hz.yueranfly.top/gtfvbmijce.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtwldcbiqv.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtgtxkmwtu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtfpiptpmr.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtbvtybrxm.html

scp file user@host:/path/
来源：http://hz.shangyingyoupin.top/gtwdqlhlid.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gtodunvsmy.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtknfexier.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gttxrszbqa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yongpay.top/gtxevuxugc.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtoubdvdtg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtetcbxwke.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtbvffgkiy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtdhyngtnm.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtxtqubgnf.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtqrjhneqt.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtbbanncmm.html

du -ah . | sort -rh | head -10
来源：http://hz.0kj1m.cn/gthqgqvjia.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtvtvvhqmb.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtuihmonvj.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtevheqphb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtovtranas.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtdvtnjoif.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gthmwpgnhw.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtxkrfgwsb.html

crontab -e;  crontab -l
来源：http://hz.zhongyouzk.top/gtglvxmlti.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtefaajmob.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtgjyklrwo.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtegplwviy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtjxnaoomw.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtznwrqber.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtymqxhrcx.html

[R70] 时间戳与互转
来源：http://hz.meibo888.top/gtzogvvbor.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtayvbeajn.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtpoxuhihm.html


<!-- 参考信息 -->