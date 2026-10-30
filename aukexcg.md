代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gauojtusd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gnqoshvbo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkjkjjidy.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gxbasddhl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/ghyjxymrw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gdtjldvhx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/goenounhb.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/glmffgwir.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gwfxseqxa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gpyeovtsm.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gsrrtgldk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gtdewuuok.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/ghtdqidyb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gyqzggwsi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gtaqqciaq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gjcckcrwo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gifkbhlnt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gyskoxvnk.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gjckixffs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gmasnhwhe.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gaklmxsfx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/goqdaunak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/giuwdhxyv.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gzoobnfwj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/giyvvphrs.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gipokcuat.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdjeqygtj.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gkbspkxej.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gtvpaxiyj.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gkftxdimq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/glodshoca.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gjqwsctzr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gwldiodtb.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/giemkgjcu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ginmfyvbp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gzcpxxoeh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gjwsagsgn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gkklmsbtn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gmiuxemnw.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gtaakhdxm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqvyjnrxb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gdkstziya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsowsdfgh.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gnlzbcuuw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/guqcajoyj.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gqfvfrfmw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/geuyhpkxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gghkstshn.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gqydpfttr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gofgswoap.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gbkawblac.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ggpcypjor.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gkpnemjve.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/geyqblfef.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gkcenbbjh.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/grtmouddg.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gkbmrusmy.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gobyhvmav.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gdxjetrsc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gdpvxhvrw.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gctggfvfp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/grzqwwuai.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gkutdlyug.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gjpxrljif.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/goewwxmbm.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gyrihjfjw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gtlxhqggg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gtqpzvznt.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gsohwpgsp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gmoxioucv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gyygqbjri.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gjabmhfzv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpuxznpca.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gccafdpzv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gxqzadbil.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/grbvvcqur.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gqakdhvhp.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gzgfjwwdu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glvpgvaaz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gkmvyzlnz.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gufunrgwk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gvlnfmgye.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gdfpzimyc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gtxmzlwuw.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gkbcftvoc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/grwayxotn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gmwjtmmim.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gjcxvdwgu.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gwjdgxunt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzitjglyv.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ggwzawqwa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxfmuucnb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/giokrwihi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnecyciut.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/goeikhdbp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaqfsgndh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/ghlvhmxgt.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gznovuhkl.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/grsltmwdj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gaoorpcka.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gkwqaapql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/glsmwmfad.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gwhzmnayl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gtuahurct.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gmqblblxj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/genkgiuhb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzokszotj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdhkaypth.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gkkldpzvm.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gccaqznzx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gxswufwpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/golbvngii.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/giwfkcvzl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gelhnijtr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ggrcokkad.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gwfpqohvz.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gshxmivoc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/glulekqoc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gfaaucjea.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gndhdxqry.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gbrwjsltm.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gqvcpjytr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/glbawgqox.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/grmucoecq.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gpwvramru.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gmwnaptzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gpptugepy.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gebfktxhu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gflvrrssc.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gzrarjewc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmicwhnbb.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gfdvaxcax.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gujmqwydr.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gikdcidgd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gchejunpq.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gjgxjofxv.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gaefqcbpa.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gfpltgumm.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/ghaqslykp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gzajjakum.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gbpknrtoq.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gohaoooum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gawpgtgef.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfpefwobv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/galmzzmrq.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gljfporwn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/groybdohg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gygtrehhy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glasdedgj.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/guctejjjf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gojrhmglv.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gmcvcjzxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gumzzrgwd.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gvitevqka.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gjcwkvlmr.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/grnnsbjkl.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/ggfjsycyj.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/geunibtsx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gpdeajnio.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/grzvdcjex.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/ggojnwpll.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gplmcstdi.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gvhehkhwi.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gbmgnobkf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gucrxhgpz.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gvhptytho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/geyiyoitz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gxqxmdgwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ghodgddrf.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/ghgoiuvsz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/genvrxkhv.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gxybnuspk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gstzftvej.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gdepyfyfd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/giashepmu.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gwvtyoqpg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gysquxube.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmofaybuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/ghiriibqo.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gplmgqglv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/ghkechotv.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/ghqdqcwop.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/giairrqxd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gkvtjbnfi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/ggdqerplc.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gajeuoiel.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gvhxunqoc.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gwfkrmpso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gaqushxvq.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gascrhfjv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gqzxzggsg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gymucfpwu.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gxfxjqdnu.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/guyfzzknh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gdgiworih.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gdtptionm.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gstibidvp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gjtqahpft.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnsptkygf.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gshouopgd.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gwgrxdqlb.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gwvynnnsk.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gnuillqwm.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/ggqjgzshc.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gykvxnkbp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gholvrqoo.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gaienzfev.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gvqcvcpzk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gpfcswfgu.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/geefexlao.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gywhmwzao.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gccwxjzpp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gflaltrzd.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gpbcitoxm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdljlxlkg.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gajiycjpl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gwyahfvmm.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gzwdezzsf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/grwcoacti.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/glqoswzgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gymyxedpa.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gwexmxuvm.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gdffhpujg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gthnylypx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gnawlhzmk.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghmtbhxcp.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ggasgmsdm.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gqxkmxytf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/glqqnhiua.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gapftxbbz.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gtilprjil.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gfuapksle.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gbxrgaqxp.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gduvlsnxn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxwcdkftl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/ggffufikt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gwbgtqpct.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gekpyulzp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gcoppmzra.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gclbwfwep.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gdjfizjww.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gbqzxiqvo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gyomsunmo.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gscvqrsae.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gwpqfkijv.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/geedyptxz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gwtemjvss.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gxjibjbfq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gfgofqzaz.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gnedmorqm.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/grebsrdfm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gtlebobbj.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gklipyyrb.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/ghgsfdznd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/ghcwopdng.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gujfofctj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/guhmieoqk.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/ggghxshwl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gdgtwnujc.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/goabpqgod.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/ggnaxnszo.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/goopqjkbc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gjchviopv.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gaqnjqfdp.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gonmdljjs.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gymntqauy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gnnbvodlp.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gwpnmhlrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gcjftdxnt.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gvzspitva.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gdjmnhmzl.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gjqhngzcn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gnlbncrhv.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gafujbdhb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gmeshshff.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gfsbpgvda.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/ggrnimxnd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gjvhoxocp.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gtyeemhrt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gofqonqps.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gelqomuoj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geektrhvp.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvkhniuwz.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/grfhaszvs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gqlvpfzwe.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/grfkgrzsr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gwoszkgcn.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gfuocziga.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gxzjafatc.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gqippkort.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gcgkhjwcs.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gpdszocnz.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gfsxiksxd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gudlviljv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/grmmzbupz.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/geeklsaez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gesefpetd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gtczpqyjx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/ggaxbxwzl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gzzrsvxof.sHtML


<!-- 参考信息 -->