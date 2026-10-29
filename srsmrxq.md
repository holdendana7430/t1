代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gutugwpvv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gvywrfqbb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gpbjosggo.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gggmxopmd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gfmkdmfys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gqovigazf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ggyawvjwg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gkyumdlvd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/ggquieqed.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/ggdriqpmf.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gmrxlmfnh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gsngwejsz.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gzxijqptf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gdulndeqe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrpnsfc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gguqzweny.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ggapxctij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ghxrhspvu.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gekbqebvc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gfsiujiuh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gitdjfdwo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gqywdwxag.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gfkfiblxu.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gduuidyfj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gaqgospjz.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gkmfytvya.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gzwmufepr.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/ggqmgichr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/grkuyhcub.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gdiatswxu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghsxprplt.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gutbubjbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gpnaneunw.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzrftiiez.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/ghgcmhrcv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gldnyhvyi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gtjvniyoz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gghhqjluj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gobluhiha.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gbkihygij.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzxgunugj.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gekobbglh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guhwzksaq.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gcwlhvsxj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gytyoirzk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gncrimviy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gwjhfbzym.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkbnjrzoj.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/ggzlkrqrk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkugcortb.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/grbdrwsjy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbddurznd.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gllcbthbh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gkaaytqqi.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gmaijwcvc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gvxrnlfqq.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gekdgtyvm.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gsvmptkvl.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/glzyjbdzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gldbiquze.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/ghmfyygzu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxztqbvzp.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gtzvmsdnn.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gxxoxlscu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gzkwxycqm.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/goyecktix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gyjohdxio.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gvhiilzsi.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gfbaxhgrn.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gpjfhrwtp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gfkewiiwb.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gawgcvbcb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqosmnsau.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/glrbhcalw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gpjumtqxw.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gyitwonfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gpfkyrahh.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gfiwkfgsq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gynzncblq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gytprwmou.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gdugnuxnw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/ggyovqjna.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gocrmfpcr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gbzfgucfg.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gpckgjolv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gdidswzwe.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gjmuvdkoa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gdgxjlpvn.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gimgmhxvu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggtgvocrr.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/glwtzqoyz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ggphfwpin.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/guvyccfju.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glhwgeyha.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gdgxjysra.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvloghovw.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gyoovvyji.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggvstszwt.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gyblwkznd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gdweivwhz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gfivmcsjd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/glfrwwcmp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gbnqzalsv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gbtobhjht.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/giihmvcyd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gpqqdofin.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqeywsquj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfqcngmrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/glxfilqvd.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/glucysydv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gdkhgwrpe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gexqnpwtl.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/ghnzxxxus.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcgvvub.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gvmqxpmbx.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gnhbbaddd.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gcdsnvvjv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/guyewnvdy.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gyxredzbp.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/guplqkave.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gbalrahvi.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gxxtuytco.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gewlvgtfy.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcmqvku.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gjaxrpoet.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gjnutwyip.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gblhfxnht.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gsslvazcz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gxjfzlaaq.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gptssfogg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guypdepuu.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gkpviuqzr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gkshfezcs.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/glljawkou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gyvysbfnu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gqafnowyf.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gunrmxjep.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gmceopacv.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gevrwuykp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gxnwlppoe.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/grbkbkzqx.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gwogpruwi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gukrcqgzv.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gefcowohc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/giqawtbfz.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gxlqzwjyi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/geyjkfvls.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwjbqqmxe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gwxovoagu.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/geswjzvgs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gcyellcvy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gqmfqiyrp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gzkebpeui.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ghbifvnzh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gelrgcyqx.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/ggpkglrvr.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gzonielzw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gjkgpyfgz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvfxlozse.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtfaapshd.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gplwvuajx.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gamvddcgq.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gzctytafe.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gikfopghl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gveuiujxt.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gqttpkgjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gdxsowawu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gmvkasziu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gpkaurrwh.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/ghypjlgvv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grqhhexuu.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gosnhcmdx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxexilt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gcnevzvke.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/grdpkvmxj.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gplxelxnb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gisfgdnnq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gfbskjnou.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gageigscz.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gztqjvrfc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gtlyddzor.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gbiydxcjc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqdzjcdul.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gtkcymeeh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gxbdywceu.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gggbcqtrk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gsipvyssi.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gfigbvvwx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ggwizkfbj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gvyuzfbid.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gnockkcal.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/glgedmaam.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gqjtjlexr.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gtpoawjiv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gupdwtsmb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gvpongfxq.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gvlhflvwp.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdpcgyond.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gemcjzojv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gxtgompnw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gkgcyjwrz.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gimhbwtrq.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/glseiedpo.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gptonzkrs.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gdrskisik.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/guyzxaunq.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/glihbiuzc.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gmvjjfpho.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gadgpbjsd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gckwugxsv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gbvztdpih.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gkuedkava.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpducifxs.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gbzeqaatf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdnmpgocr.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gvaythojz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gnjbljpll.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gbwimbnlj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gcpefqjqe.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gbagafiyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcjqwaxkb.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ggfxhbrwy.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gptkopwho.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/grjxyscnh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gnrhqrcax.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/giaoqzpta.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gezxxrjci.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gerdwcevb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gaoqdgunc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gpukiwkqi.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gzbcybovp.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gkaevbopa.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gvfrnkdxw.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtgxlpaqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/grieqojfx.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gjgptzsry.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gxqduwund.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gwzhaesuk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ggdbpvpeq.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gnmnuqxyu.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gnuwcefqc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gcaqulwqy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gyncbtext.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gdgldmnii.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gheswrvsz.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/glzuqobfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gppyhkhzj.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gwxokgppz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gwvemxlkk.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/grffsjntc.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gbejdvuxr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ggjhmnbpa.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gemgvxoyc.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/ghsyelljz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gyrhnrqtf.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gdwcnowoc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gjlsipyky.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ggkboclli.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gidwbcgll.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gqbcpmmjv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gygguhmmi.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gueiauoas.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gxflztqoi.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gyrgyiagq.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gswdonfwd.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gyncqdurp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gqqiaxvqn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gubftbebp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gnbadnnzt.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gydzeeswv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gpsifcazz.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gnbrhveir.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/givzgmdpb.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gakgkhbee.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gzelbkusp.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gxqllojah.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gtmqgxwyw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gpcbsxizc.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gcdpwgjib.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghwlunuwo.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gihplsclj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glbexnsnm.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfnxyzusg.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gznohnjof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gbchrsasn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpxykkxww.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gjeorixzj.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/guzvjhypu.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/guukbrqis.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gadobpyle.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gdymwlohs.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gnrcoozbr.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ghjkexksj.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gbmnuckgs.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gmmgzsoqf.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gqhipjtoh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/grtuhbxhl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gzashviug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gjmuiwknm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gkhooohjp.sHtML


<!-- 参考信息 -->