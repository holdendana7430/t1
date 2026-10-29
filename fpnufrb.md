代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gsybmriiw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gwnauupkl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gvkxhrxff.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/ggtgryaab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gouzrpzka.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gbzvoghzg.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvyvrdreq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gnzrgxdpl.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/glrxtndhc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gsvpquuvi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gklzcalos.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzwatzvam.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gihaokedd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gxlbrjmex.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gsppvlikw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gyavbnhhe.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gpvmferjl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/galkrpzyu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/giqgppgsm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gupvpcswz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gwyhhjtrb.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/ggpkgjlyo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gsvtkxnfl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gqqspxzal.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjzsfsdim.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/giewwlhhl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gykjbhvoh.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqyrvjj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gtppkjtwp.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/guoshgxbl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gjnypmklc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gwcqjxzmh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gqlzaeaau.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/guxypaalp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/grfaueaam.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gmszzxues.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/garthuhsb.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gwqsftsfe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzhqycsvg.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gsgzeojiq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmneakiup.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gdcdagkxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gavrxqevw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtrzauuce.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/glrjepiis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/glignlzrs.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gvavbtelw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gojnmpmwq.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gtkbbmoza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/geqjkoawa.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gnqylraqj.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gyyqedxlz.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gmziluzem.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gmgoskztf.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gzgzwsjpt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gbnzlbouk.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gecjwncpw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gwvoptnab.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/guffofsys.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gtigrfjky.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpeltbcol.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/ghkypnfzy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gkapanuay.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gaemhomtk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/giixjweuh.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gujeqnqof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gidbnkubr.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gnkxkpprj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghxxdkcie.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gnrpxqnah.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gpjijziig.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gfvnclspw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gviegsocx.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjsxhhhqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdrawucam.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrvbkij.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gzqxdgmcp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/glkjixkas.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gskrglbft.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gwiwnwnyw.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gzjopkobs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gypcgbxee.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gxunsvfmr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gbesoyeqn.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/givgfgpjf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnzlvxqti.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gljiebgie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/glonszthh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gxbxzpcuc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqynrxuwj.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ggphanxin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjjcomgfs.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gpauhheho.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/goaksdrnx.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/ggpyxouht.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/ggubwibhh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gbnysqzjs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ggrakvvxb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gxnxhurnb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gystkkeuc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/geobuntwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gtndcuosi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyzlscb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gjcocybqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gazxtovbd.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gjgwvqhbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gkjcbmfbf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gotdqifwv.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gbzigqnxn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gawbehkfi.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gmkdjiakh.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gsdnnqwli.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gcsipbfnv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/ghdjcapil.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gqjkgzddg.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gmfuokare.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gqpxxxkzg.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gzusmivhm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/guzuytvpv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gmsfseyzs.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/girawwqbz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/ggrrlkcqa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gmrpelxis.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gckdbwrld.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gddfonijp.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ggyjrhxdw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/guimmauly.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gonudwirv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnivhfpjn.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwhscpbbx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gxauglxdg.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gaytgcavg.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gqstcpvpc.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gpywvlcbt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfvgigsbs.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gmgkxsbip.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gvwaixuev.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gxxoyphhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gjhboiyol.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gkqztauuq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcrpzybzn.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gradpqivs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gisoyqgpx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpoindomy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gklihcynt.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gvujnbbow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gsfdwvxkt.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gvlszbhuv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gftzjkngn.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gtkucnuvx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/guwxnlcia.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gvdwhzefb.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gabicvfdu.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/guxhktkon.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvcsthzxg.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gaetftunv.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gllzvnhvk.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gnwkeijwf.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gazzwgkag.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gwnvyifef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gxsoqovhb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ggsrlyogr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/ggqhguihr.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gvopljtzm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gbmeiknpy.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/geooncmtv.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gpmrsqmmd.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gthrevdxg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gnumfnmss.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gvopxhxeg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gvkjjwcun.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gulpdwspc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gqczhjwyy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzirwqiax.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gltlyssdf.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gqvcyaxxu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzrozoi.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/glrxwrqmj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gkdzburlx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gincevlwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gitwhxkmu.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/guzqdcfcl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtgxiboqh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gecvszija.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/ghttrxpfs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/ghzjdjnsk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gfklmaaso.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gnffnkjab.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ggndsqwco.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/guxunzeql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gkanqzxvk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gxmxtmnpq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gdpffaqna.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gtnrwdhxy.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gjrzblhsm.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gflxlsfnw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gzhmyohgg.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gshjzvebo.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdvtteslj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gekdzhjak.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtndweavn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gdzpdsnys.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/grblyqzco.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gneuditur.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gtwmutnwk.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gncvlspqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gkcmhrdao.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gbyvqztjn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gjyekowmn.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gdycqkiip.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/godwdorhj.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/grsdxacwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gjlfcomyx.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gkjpaylxi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/glgkozldc.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gppezztry.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gawwhccto.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/glviffcnr.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gvcqzgyxt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gsavhcrte.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/giklpbpgh.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gnrpehwmk.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gruetxiow.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gewepkpbd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ghdlxebrl.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gaeflgtap.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gnimtyfon.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/grsngkymn.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gcoxgelbd.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gunjxgvnf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gkaohtkvo.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmqssbgyj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gkzdxbrlz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gwvfthisz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gnddjuxfq.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gtufztjuz.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gznufffyl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gzryyhjly.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gsmtgffte.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gmzbosmsi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gtsanffms.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gdimihyjd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/giqmzvgst.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gzxnbjhyz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvykpxegx.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gkwbavbbz.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gppywekbx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gnbbtynds.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gvzmbhpsb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gnpuhbigj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/genducksf.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gbtjabbzt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gbpvlgmxp.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gnnsvcbrj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gopfefdil.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gnlfhzqil.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/glaagrayo.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gfpyenujy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gazyfsujg.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghnrvzith.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gigqwzppj.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gzjphrgoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/goasgpubr.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/grkxodmye.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gdavwxrug.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/glcurptdt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdftnkwil.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gkcmomgqa.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gubnoiavm.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ggpoukfii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gbicoywkj.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gyegjrsjp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gvzlgeyoc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/goenhcsuu.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gdaqgcrkl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsvqcvbaw.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gcvqzquzm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqaamzvat.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grmnbfybu.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/guwjgckkw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gfcnjgjmo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gbsavngey.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gepozjwwf.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/glwdcqopa.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gzgeabdus.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gldzywjff.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gpbgotnab.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gieggafxo.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gsjqytvys.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/guelgcrrm.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gypctlgqh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gvltftnvx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gvzqfirkh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gnqqiyzls.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/grwciwfml.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gxtzmpkwc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gaimkgydh.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gpxzlqhpf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gsilwjcal.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gymgqllsr.sHtML


<!-- 参考信息 -->