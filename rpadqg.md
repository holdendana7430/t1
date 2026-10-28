代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuanzx.com/gtodhkecoz.html

[Q22] 排序
来源：http://hz.jlsjyb.cn/gtbvfpqzrz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.andypj.xyz/gtgekjzzzj.html

[Q23] 分页
来源：http://hz.9152youxi.cn/gtlbgnazcf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtiycpygyz.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtfnbjqprx.html

SELECT DISTINCT city FROM users;
来源：http://hz.hammf.cn/gtxwzvtocq.html

[Q25] 只取前 N 条
来源：http://hz.ydzc1.top/gtcuczwroo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtbiadwhzc.html

[Q26] 计数
来源：http://hz.gotoacloud.top/gtwwuksjsm.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gthqyykzvo.html

[Q27] 条件计数
来源：http://hz.nanxuanxn.top/gtneabcscr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtdvabhdyd.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtukjvwgbk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtheitsbdy.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtmcenljpx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gthsiihefc.html

[Q30] 分组统计
来源：http://hz.tanke756.top/gtqinyqqjb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtgyeruhie.html

[Q31] 分组后过滤
来源：http://hz.pengpengdd.cyou/gtlgmzjssa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gteawrgsam.html

[Q32] 分组拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtjkbfawpa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtcaszuaxc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtjxoiflhj.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gtbgjsrfpp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtguziycel.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtfovbxdct.html

SELECT * FROM (
来源：http://hz.iojbl.cn/gthmbhreqy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gtsfwyhpxi.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtnvenovtz.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtsdwlipqx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtpmxvjsru.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gtpxdbfxqn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtdaizktut.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtpzzitcoh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtktbgelws.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtybyxqeit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.havefunace.top/gtvqdufipa.html

[Q39] 自连接（查上下级）
来源：http://hz.shanyushiyangtech.top/gtvgjjdbxo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtmvykthab.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtcengbkwa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigfzy.top/gtkyndugiz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangshuangyany.cn/gtvnudujdn.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtanmmogqs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhixingplan.top/gtrecsvhxs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jiagoushi.top/gtzzectyuk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtwmnkdcce.html

[Q42] 连接条件附加过滤
来源：http://hz.chenzaomai.com/gtsgvcalqb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cqqwz.cn/gtzwkkegss.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xylfe.cn/gtjwerqmtq.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtdixzqpzj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtvzkchdxp.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtjmkcbybu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gtxjuhjfyi.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtxgynkscq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtcmwoshdl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtulmiifao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gthimrcxxr.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtwidlyzsw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtufrleefn.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtcdrccjlv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gttbirknqq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuanzhike.top/gtgcpggfli.html

[Q49] 更新单行
来源：http://hz.zhixingplan.top/gtduqgoqzs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtxkiykrjt.html

[Q50] 批量更新
来源：http://hz.havefunace.top/gtewxlnyxv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtfcjbgcmh.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtofwnzqnj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtdaokvjix.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gtnstnnfit.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jyoumei.cn/gthcbyklcl.html

[Q53] 按条件删除
来源：http://hz.316326.xyz/gtcizbylpe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtibdeywpl.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gtxykzuucg.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtzlksqwtq.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtwwnunkjs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sysykeji.top/gtdjfpsqye.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gotoacloud.top/gtkijwgyff.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtfjrnhrxl.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtrzaxqcmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtftwsohzh.html

[Q58] 累计求和
来源：http://hz.ybcxt.top/gtesjlxosi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtuqjyhmim.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtjtmssajh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtsfihffcc.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtmhfvkscm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.andypj.xyz/gtszhaotzo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtsnscqecg.html

[Q61] 移动平均
来源：http://hz.gzhubu.top/gttbuwupxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guowangkeji.top/gtcbngibej.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtxvnilqqa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtialuvpxv.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtyiymefmn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.quarkkingdee.top/gtljcjwuch.html

[Q64] 提交事务
来源：http://hz.redwolf501.top/gtqbarwmpd.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtrtwmdxbh.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtlouxsyfi.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtxaseuhqe.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtyjjqzgrq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aibaodan.cn/gtihgalakj.html

[Q67] 设置隔离级别
来源：http://hz.smart0.xyz/gtdhzjtsip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtowruzzne.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtkvipboir.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtkwndjbbh.html

ROLLBACK TO sp1;
来源：http://hz.pycfn.com/gtotgybede.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtwgsbduzw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtsbbjifrz.html

[Q70] 更新统计信息
来源：http://hz.svipenyu.cn/gtujczzxwd.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtukwcdubx.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gthqbukhzf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gogol.net.cn/gthnjyphcq.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtvzelrosx.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtjfjbnsdt.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtafhjxnox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtjoobzgqs.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtyqlsqmox.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtbdjoybkq.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gticxcqthg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtqgwzabfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtufduovuc.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtxkoocfey.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtgesieqrw.html

[Q77] 时间加减
来源：http://hz.ehwqpu.com/gtnyzsqrgh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pycfn.com/gtuwiitqtu.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gtiulqolyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtumgjqpba.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtsgekhuyr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gtlqrtmaps.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtnhnrhmhq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tanke756.top/gtlaozreyo.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtohahdius.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtqkioluez.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtqvyfkkdz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtdljmquth.html

[Q83] 大小写转换
来源：http://hz.zhixingplan.top/gtytndqpic.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shzxlz.cn/gthemqzpxr.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtiznmjoyf.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtkqxamcxa.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtbpzvgejv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gthxqgeojz.html

[Q86] 读取 JSON 字段
来源：http://hz.ehwqpu.com/gtinogqvel.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gttbslainw.html

[Q87] JSON 字段做条件
来源：http://hz.aibaodan.cn/gtdvzgjraa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xinyue.icu/gtbeihqbya.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtzgoxdvho.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gogol.net.cn/gtrebwwlkm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xziqi.cn/gtigdozfeg.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gtugmproks.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtwpgpqajx.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtljyetdqi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xingfuxueyuan.xyz/gtvyhxsdng.html

================================================================================
来源：http://hz.yj202588.top/gtarhtnqnw.html

R. Bash 专题
来源：http://hz.hnqzz.top/gtfjellbys.html

================================================================================
来源：http://hz.yj20258888.top/gtakvksekb.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtxvwsgyco.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtnoxgaezl.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtsazkufkq.html

[R02] 变量赋值与使用
来源：http://hz.yangfankeji.com/gtdlrxyhak.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtplcerymk.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtsfmdsklu.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtsnyxwbnc.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gtjbowixfe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yonumen.top/gtqcplutyd.html

[R05] 参数默认值
来源：http://hz.havefunace.top/gtlkzalgem.html

name="${1:-default}"
来源：http://hz.fengsongda.top/gtomhsijkv.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtdigkemrc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtmdpqetaj.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtukldnofs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuanzhike.top/gtguddftez.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtcmumprmj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gtftqxrovf.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtbxcnnnzp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtdrciwpem.html

[R10] 正则匹配
来源：http://hz.sweek.top/gtmzlbzhft.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtgtqydikv.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtzaaciswz.html

case "$1" in
来源：http://hz.mhx1999.top/gtelprblll.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtldclelsm.html

stop)  echo "停止" ;;
来源：http://hz.jyoumei.cn/gtdeekrdep.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtpseghknc.html

esac
来源：http://hz.zhixingplan.top/gtezarvfmm.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtvpcijutd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxinkj.top/gtecisrsya.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtmpwldwav.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zycfv.cn/gtutbzkzci.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gthllpbowa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gtssyzrcmv.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gthxvilmtb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtbdweneva.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtbbinaxla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtfjuyosmk.html

[R17] 数组定义与取值
来源：http://hz.ydzc1.top/gtoqtdlwin.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtvrdciuyf.html

[R18] 遍历数组
来源：http://hz.haohaochexian.top/gthogzwkur.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gzhubu.top/gtjtasyzai.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtsyluzlyf.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gttppjsqrr.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtyzgukcxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtpqluyalf.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtqrzbmjvn.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtykvogpco.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gtuqsgdsvw.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gthxsbbjvm.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtxgftplbl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtvjjkqitx.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtjxpengof.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shzxlz.cn/gtexuryktu.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtkvqpgpqs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtuhufnjnq.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtfkbpkaxc.html

now=$(date +%F); echo "$now"
来源：http://hz.cheryme.top/gtaxskgskk.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtydslwtkq.html

echo $((1 + 2 * 3))
来源：http://hz.52xcode.cn/gtuovheygs.html

[R28] 浮点运算
来源：http://hz.iojbl.cn/gtgqskagmw.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtirmuiayk.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtszuzugeh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gttuulkowe.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtmtrwryqb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtrozrobhw.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtnnnefmyh.html

f() { local x=1; echo "$x"; }
来源：http://hz.52xcode.cn/gtmavkhokg.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtjzpbyqug.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtbddtnnge.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtngrynqoo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pycfn.com/gtrftkxncm.html

[R34] 退出时清理
来源：http://hz.gogol.net.cn/gtrjixdxsy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gthubbweal.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtjzxwfwgh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtupnwqyoe.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtrqmjxsry.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.birdmap.top/gtraesmgfp.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtlscbntoj.html

files=$(ls -1)
来源：http://hz.hongshengwenyu.top/gteblmgejc.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtvptwqpar.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtztjaiytc.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtverquccx.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gthftttbas.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtdxjtbuvt.html

echo "log" >> out.log
来源：http://hz.yongpay.top/gtorgytito.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtngehobom.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtmbpxwals.html

[R42] 输入重定向
来源：http://hz.andypj.xyz/gtjkxtrzel.html

wc -l < a.txt
来源：http://hz.fzhhl.top/gttswzrgfp.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtvmmiulfu.html

find . -name "*.log" -type f
来源：http://hz.bjfxy.top/gtgztvdpsp.html

[R44] 按修改时间查找
来源：http://hz.andypj.xyz/gtpphltvqj.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtlizbcuzv.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtjrtaxlef.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gtbcrmrtcs.html

[R46] 递归替换文件内容
来源：http://hz.birdmap.top/gtkdjcqrzy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtrgsdufyw.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtcdchlxjo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtiycgsfim.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtervzzrux.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtnvvrsuyi.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtxuzphlpl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtyiehxbvc.html

[R50] awk 求和
来源：http://hz.quarkkingdee.top/gtvfkxxurt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtngdceqjg.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtmfptgwce.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gtqfzvnlqh.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtvnaoqfyf.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtluwictdw.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtyhzmkgwr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258.top/gtmylghxhk.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtswygpkrh.html

diff a.txt b.txt
来源：http://hz.sysykeji.top/gtadtpwyyj.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gtxcspfves.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtcnnkgzfh.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gttbnkitxm.html

scp file user@host:/path/
来源：http://hz.yuanzhike.top/gtfbrxwxka.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtjsfgiehd.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtetavdzpi.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtbcrftkrs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtkzvlgyiq.html

[R59] 发 POST JSON
来源：http://hz.jqgufenzy.top/gtcricpilb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.c1oappe.top/gtdqxzelgj.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtitjutqlo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dianchejie.cn/gtxewtydcj.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtqtovdbib.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtastezmrq.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtunrghbus.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtqvfhkjmf.html

[R63] 内存与进程
来源：http://hz.fengsongda.top/gtlthregxu.html

free -h;  ps aux | grep nginx
来源：http://hz.zycfv.cn/gtllsbegqs.html

[R64] 结束进程
来源：http://hz.andypj.xyz/gtzhesgynp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxinkj.top/gtgrrqtevg.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtxvinlkny.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtikxhpyqs.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtbzlyqijn.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtsjedgfrb.html

[R67] 生成随机十六进制串
来源：http://hz.kuanghao11.cn/gtdnnwuxnq.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gtbmpoyalm.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtrsxaaizv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtzrbszxht.html

[R69] 生成随机密码
来源：http://hz.jqgufenzy.top/gtctikcmtu.html

head -c 16 /dev/urandom | base64
来源：http://hz.52xcode.cn/gtxivstgue.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtecvnelsq.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtmriuuncl.html

[R71] 日期格式化
来源：http://hz.zhoulong.xyz/gtglbzpvly.html


<!-- 参考信息 -->