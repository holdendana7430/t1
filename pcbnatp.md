代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/godzmgspw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/ggkdbiygc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gqshlwlee.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gsbdusods.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/geljfhinj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/govkzqhxm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gxegupsth.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gpjhtzdog.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gotcpzhva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gnpahyhee.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gjlizfpxv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gmotssnau.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/ghkftsykl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/guvkzytfg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gabsfejlt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gnougjpsi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gfaupijgv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gbyurreag.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gmstrquqh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gbqozsavr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gcbiajvii.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqxpesxlw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/goblhntem.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gmzzevaqn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqcnwofdm.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/glofycuwq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gyenvngib.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/glfztdnky.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gzoexlyhr.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gpsgaaqqk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gqlbhwubr.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gmarlgnjm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/ghmnhnvjj.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gdzrccdzw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gthvjbtjh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/grmouadtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gcugsytar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gfcdgzsse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gzirkllsh.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gdwgxchqs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyxqelgyb.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/ghhsxewkh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbmemyajj.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gyyuwyuey.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gozpddctm.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gdhwcyvae.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gmmlgfevv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gadibeucv.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gzsdkahlh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzdgjkpsh.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gyagkeoss.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjfecddit.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gxxbcpxur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gzevwxrqp.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gugvdlvmo.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gvtcunntg.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gnzhnglhs.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gawkxcnkv.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/glxpnxgpx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/guotvqmrj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gpndofwqu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gnvzuqpje.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gvrcgnsgt.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gxraothul.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcjlblgxi.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gvvabjmre.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/guwrfupso.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gfodhsebz.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gyczptark.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ggkhdhltx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gyelfbuku.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gqynoecis.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsuxzxvqt.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/guezstbkz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/goryzujrc.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gsxxjvqmx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ghekzilgf.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gaobetbtp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvcfzefci.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gzrdnrrgw.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbkzodcaz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gpxczbbmn.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gplkxbnlp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/glmetmrst.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gjlzwhrms.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gvvpuvzzq.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcnictfes.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gratczgad.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gdrnhsqrl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guwqidfno.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gollgvicz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gniyvbvob.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gswhtfmbm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcufwwkpx.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/glqesgmmg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbrqimllr.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gralkwrbt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtavmrwke.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gllwlvhxa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gxaefgzwk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gutsmrsyl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gunxnxoil.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/geltexrmv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/growdbyqh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gbjfejgqs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gwhxawwfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghirjpenq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/grufnxtom.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gitghrefo.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gvdgdbwcz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gzzoyzjjj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpsmrgkgc.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gscqbdtia.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gojornjgv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gprwyioca.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gdjtaagsg.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gtwymeluf.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gnbbvugku.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gopbqvihw.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gnskcffen.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gyygtufai.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/ghjhtlecv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gccpmulcn.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gwvxuohst.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gpdbysabm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmlgcuiud.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvmhgqoil.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gnesjzvgg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gbyfdxzhf.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/glvgzhvup.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gvsrlibls.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gnmcmmlyt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/grgvfcypf.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gvorooakt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gdartnpnf.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gwkmeqbky.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/grqdphsnz.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gelacwith.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gfzmyoqbh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gyphyavwo.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gwdauqjzp.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/glanfwhsb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gufjhyqwv.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gvmapucrv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gowutisdm.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gjnndkijo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmahaenvf.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gocltpumu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gaiuxbevh.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gvwtllfrx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gqfndcmhh.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/ggakxkxbf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gdvequbbi.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gbvcwbwnb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/ggluhgelq.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/grhbaqrhk.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpfspdhif.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gqazwgggk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gpbnoywvz.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghzqlxsor.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gbwfikwrl.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gfwarfhti.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gssfetyuu.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gvewzyhkm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gbbuavasm.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/guzqqgeey.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/greedrfnv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gcpyldgar.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/goupuxvna.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gnlhihtlu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/grxfbadnt.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/ghgsdrjoi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gjtyusdaz.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gkijygmre.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gykktzywy.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ghpodtitp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gymjmlmdl.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gqcpniofn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gphaeftxz.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gozofmfkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gpkkmxxuj.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gkdgdzekf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmrhvndxm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gsetdknqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gzvtwgalu.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ggyqzgvqk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gaahtuhmr.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gdinxlala.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/glgqohvhd.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gnhamfxvz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/ghgyhsrkw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gtedzjllu.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gbmkgtkpt.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gyfshxnhk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gihnnhvji.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gwimscccc.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gzezgdzwk.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/glxleuajj.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gkeofboev.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gyickjlon.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gmdqcpktr.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/grxymvyvb.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gpdwbujyu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gcotanzmh.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gjnphrlwq.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/grmupwdhp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/glssnnisx.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/grwhatyqb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/goajaxgdc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gccvwdgvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gsozntsfy.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gsdeelvob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gbaaunjir.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmpwutkau.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gyyksvael.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gikmpszln.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/goslorydf.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gdmezsbce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvjyyyaft.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gdsgoicio.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gudbqcntp.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gxbvhoafe.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpwogdivk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/glskndncq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gkqnuztsz.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/ggqhkbgvg.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gpguzfary.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gjvmhpaod.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwnrdlrjo.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/giicfsfpd.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gryijvgat.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gfzrbxphi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/geyczwkpl.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gxkcbqkbz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gpxjzavnz.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkkiimdef.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gptbkgdip.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gvhwipyrw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gpuruxkwk.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gcmkwftmz.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gcnvncacc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gybkqgrub.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gatfwotpp.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/ghemitvxw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gthqbqhyq.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gejrlclwt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gutmhuuuv.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gecechhme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzrgnum.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbmvlfbbb.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gxpndlkcc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gkrsbsdij.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gucukpazt.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ggteygusy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grgxsoaoa.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gshqojjbj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/glrivsjei.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gjpdapmgi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gzlrfdyvo.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gduibhrew.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gjhyrmwos.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/giyomgdjx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/ggixpejji.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gxgswxfax.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gaeupxcmx.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gzglngtkp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gtnopxjbl.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gcyerxrvu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gzrxytewp.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdriwlrhe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gofmbutui.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gftytevps.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gjkihqlcs.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gxksckzvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdnedwlbo.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gdiewrawc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gcllrevtm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gmfhoqsep.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gtalytyvj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gizqssdwk.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gsxzmusdp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjjllwafl.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gmoaybnrh.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/guqazkuak.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gmlgivtsf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gktmtzgbd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gmklcxjxw.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gmogcamsm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gloqmtsht.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gdemumgpk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gvgiehzxz.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gsbebhzdu.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gnzywjkfo.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpafswvay.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gwaxaucvq.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ghrqgdhaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gwzxduumf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gaeezynjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gvyhcyjoy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grxhkenov.sHtML


<!-- 参考信息 -->