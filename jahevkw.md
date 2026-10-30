代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/grnrdnlde.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gqnjttvrs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gfhvbqfjp.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gxiuiblzf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gcmaoruvt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnnwoav.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/glsrmrohb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkfoknczu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gsoefvllt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gipuwyoiq.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gujllecax.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gymlbxmlq.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gvnngqkra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ggpzyqmvj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gxjeipdan.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gzrxteyrg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gmsjwfwco.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gtirzzbqf.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gyfhxajtw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gxnfuepzy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gnpclggdj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/grnbkwlfs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gyrftkved.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gkwdcxazr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gpnkqysnx.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gvkbcnowr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/giwdwagdd.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gxuooaaef.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/ghrpretxv.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gfaaxevry.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gyzjpwhfe.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gccwgirjh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gwaovrapy.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gkhczqywt.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gixfpyqxr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gzwgnevtn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gjsgangvf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/guhbvaexc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gsfbmqgpa.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gicpwetib.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmyfvqifp.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gyspmpamb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmpzrbcia.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gnywjipyo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmfxxxyiw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gmeikqwxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gzgdpeshg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gucujspdn.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gincpzmko.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaxxvnngz.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gcuinxzbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyfuejooj.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gjlhhjokw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gliysrpis.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gtntkbhjx.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/goggfldrp.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gngjjonal.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gmyeormgr.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gzzucfltr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gqtsfyqql.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gdsxuemus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/grypkcroo.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gprmmyieu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gimrzlguj.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gbeyblvni.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gdexwtfhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gmzdxxaab.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gyrcbppzs.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoeulnsa.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gkagjtuhg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gfattdpmp.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gvfmkcgph.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gmfjgzlgd.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gpeytmmig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gpvifjfgc.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/ganqbfguq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ggezwtgxb.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggyhnxlnw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/grehrjhcl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gvgnqdzaq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gioybmaqj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gknrtavkv.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/geuuqjbee.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gkuijoowc.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmbenxeno.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gnpmhzcpg.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gvtaemjwp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/ghpwygkim.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghwskdepc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggwovyfrm.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gnzsomcdx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkkgwmauq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gqgekkkfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gunobnxkq.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghzgiywja.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpvsxjitl.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gmujbqfxy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gupuhttch.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gixrhqoxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gpufuzras.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gansrbhch.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gwqkkkeax.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gvpzkvrae.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gckrsqdbf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gyocbdwax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gaihtokhq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxmmfdtkd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfmxfpnxj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gpeqlnrhq.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gabekkjsi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gnkmydhqd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbnnohsat.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gpjisttva.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grkzibshn.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gnesiennm.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gelltjfgz.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/ggxtnlisi.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gtmqwzqtd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gjtntztot.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/guzevrlkt.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/giryzrhwo.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gqnxrwfwl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/goofbnclf.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gsdcvlsac.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gquztuivu.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gguswlkxp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gllhmhaom.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gogbwitje.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtqknicha.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gfjbroptl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gdrcubkre.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gvrsyejgc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gspgyqugs.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gixjzbngv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gbfoioagw.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/grjhljxry.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gsdzfeyip.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gyoyxykux.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gnnmlbtmp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gyzidxjxa.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gthadfqha.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gcjgmkcov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gzgejhcjk.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gxxanlgds.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gctppjjrc.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gcvseghdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gvuqqqolt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gujvbcquv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxsdrizru.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gdngetlig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gjuhxdbva.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gcnpbsfse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gcjeogmir.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gomarwolu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/grcneuliw.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gdjbghdtz.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/girvnquot.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gcyebiwxz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gzciqfmnc.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gznfventi.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/ggmtkglgd.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gkzsdyipz.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gsmuzkdko.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gmqxvwddn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gmecxvugk.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqmbrjwyl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/guwvbnczd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gvzfppbhb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gcueoobdz.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/ghudnffmn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmkfcan.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/grmxyydii.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gbvpuscgx.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gtualptuq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gmiimffev.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gyqynhuih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/goskzwcvb.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gwpjsfctx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gzmjtyajs.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gibxawuad.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gjkvjfosm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gfwegesul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gcrdnnswm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gklcknuqy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/giauehyhr.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gskrywuil.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gsvwxyffx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gmszzkoik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gsahvysld.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gmrlgugjz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/grdhyajnq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gxmbonvej.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gchugsgtq.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gvmrubwgh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gsfwviajy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gbrhfiuin.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gljmqescd.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gdacxkkuq.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gthphmdcl.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gvonuzvnv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gfbjoknbo.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtggnrsfz.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gbeuiindo.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/ghjpnvloh.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gaaobrdgr.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ggyaekomx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gkuevqqtw.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gdzcoahwl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gnpmdceku.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gluuitwjd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/grjvqacxa.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gplvgjvpi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gjmnytrbs.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gmxfshoad.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhtvval.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gpwetmgst.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gfxgdjgyi.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/ghngxbqxp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gigswojjt.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gndmwgzim.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/grmwkgxzx.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gjiwijhha.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/glmnyvcvm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gzhowxvay.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gwcdriobb.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/ggryadirx.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/glatgjqqu.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/ghrqeuvmn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gvaasmiba.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ggpwacmbi.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gslkdvkhh.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gjlsgoznp.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gkjoqpgvg.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gyxkvhcon.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gaqmpfdtn.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxocszdkz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gdyxlvxce.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gmujuzmws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwtainuek.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gftihuqin.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/glhubvcyi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gvziupcor.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gsbwlqhjh.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gnzlmsvqf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkhpnbrvy.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/ggcjlwnyj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gvixggyup.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gxxtnwsfw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gxtiotvlt.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gpxjymlfx.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ghxqaljni.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpgnjnf.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gqtnenbll.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gmycklbjt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gznbuceaf.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gnyxurlug.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/giecmnyiu.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gsmisweuf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gyfrlrmvw.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gjdsljajf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gogugiipk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gizehtmeq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gghbxmbzy.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gpiycaeqk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/grskxuiff.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gukonjrvn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gamxjpbec.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gvsulqutc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gvfqprhkm.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ghfrcizuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gergbybjp.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gqepuqnxo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gwjjgvent.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/ggbvyeywq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gsofovdft.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gofzhpzmg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gmzigkxen.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ggylvfuln.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gdcfegbti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glczoaugq.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gmfyrwiwd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gilyfaakb.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcyyjvpqj.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gnacgoryt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gtafiobly.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gkkhhrdba.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/grqoumbnz.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gdtfybktf.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/ggjxwrobw.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gpejyrrho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/geydgtcgq.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/goqslzsjm.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gviggkytf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gxwtzukcf.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gywehfaok.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gkikdjbnv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gylqcjcuu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gflcsbwld.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gmvutlwho.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gpgyrrvrm.sHtML


<!-- 参考信息 -->