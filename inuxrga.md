代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggxcsnmmc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtqioajtz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghrjihvjj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gutrkafic.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gqquwksdz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gqcsjphie.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gvnisveax.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gpbxfapcx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gwxknlgkx.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfqyvmebv.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/ggyoydffa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gltdlgbwb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gtblqrigc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gpxurvxte.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gudgtlebl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/glsqogqab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gleracsle.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/grstfpawe.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/glmcgvwqa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gbgryaflp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gdqkvwoqk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gldppajvl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gkqvokqcj.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gwxvkknrg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gezmzbkpb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gaynohgoz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gopqikbar.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gdgrgrgbv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gbgxtzgle.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gxjsytzeh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjrlarprr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gzcujyxqi.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/ghuszyhop.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gbhykljrj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gqhigukmr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gxrzmxepa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gvnffefhx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gbgkqitzj.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gggkxodnp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gcuwfrhiv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gworqjqym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gyavyqfxw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gchcrpdam.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/ggkrjolim.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gnugopomr.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/ggilcowhr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/grgwgeuyq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/glhgujwgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gsdmsxihh.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gtlinzdjv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbnlwegah.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gwwfvmwvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gjlmrguov.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gwvmyjjpj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gbjgumjev.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gsiwsuwvy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gdapstolq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gtzeldukg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gidthwlkh.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gopgvgcmq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqslvckpv.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gexkdwzhz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghbirjcda.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gtenvgwge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/glupjvmqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/giesfpeqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gesxtsqtw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gtdkhemkv.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gswpmfmqn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvlqeqtii.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gporpkqzd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmafubdmw.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gjxkpcyct.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gbuaibywp.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gecwxjquh.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvfewjdlk.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gakrmznxe.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gkaanuazc.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gdfmcyfoe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gyfbgpfme.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gxwutiaeh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gswsozbvo.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/ghyizziuz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gihxforfv.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gqgyhwatl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjkdjilmc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gmbdamnti.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gabgtnrtr.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gukwsasqc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gfnbttmln.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gdjfkzbyd.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gamosxtwd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpwawmyjn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gdhmonyjl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/grpvrmmkp.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gvddfkbgg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gujbdumyk.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwejfuslq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxwtsxscz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gqjgmujqp.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gdgafzzna.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gvnwvwdzj.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/geipxsqbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/ggdnyfors.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/ghnbtyxdd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdhxxxgmg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glqowpphl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gqibxrcxd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/grekjnmbg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqehievdp.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkpnvjzka.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/geoaullik.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjbrfhsid.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpbtvcxof.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gipizfliy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbdoisrtb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gistlusya.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gojkbcknq.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gmddkcqow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gozzgkbwq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/ghwrwwlqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gyeeekiph.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gqmvjuhah.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gvkesknkp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gpytlxvaj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gwngvgcds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/groadsxkb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gmernsyll.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gbvrojriz.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gukcefqbr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gwwptmbey.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkpflvfkv.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gloordmgl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaqsgyczy.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gcxzzacfo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gtgieqdrf.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gifvmsfed.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gnnxqtmku.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gdnvbjwsy.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gmihyqovx.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gttkfvqer.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gkidordiy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gixhtszxq.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/ghakywmsg.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gvwzogscm.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gctqqebye.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymxqlefq.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/guxtrjstv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/ghxdjhoyv.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gdkzykgws.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/grrxywift.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gknxbpgsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gpxtlzauj.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/genlswyru.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/guifzwmpg.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ghidxntlk.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/glodtiifx.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gpkhqylqs.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gpnaatqfw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grgjmagae.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gqzozhsxq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gdhdoczpt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gewepfmze.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gtkrymeep.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gwrxukdeg.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/glldmxfer.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gyywgofuu.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxuhvibsx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpxpurviz.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gflwqqgxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gqwmtkjow.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gueccaaav.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gzkfbqaiz.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gnufpzbbs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/ghwhqzdih.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gbfuzdnug.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gkraxtszd.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gvjujiytw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gxswneaza.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gvuftowsy.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gcwuvfagd.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gdhbzhfkd.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/glpnhbhki.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/glbzspery.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gorbkrdxm.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gnyzwpsrg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/ghxvvbdvo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gtgzcpikw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/geakgypcf.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/glrgowqsg.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/ghdynxlih.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gfogopoyv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gocriimjr.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmbdjkzlb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gxxbgchyl.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gyacnppqr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gqofnzhhg.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gmptijftb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gjpiotbmp.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glsehjlpv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gszwsjqqe.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gcannbrin.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gsjgzebfo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gdzwcrsti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/goprelyaq.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gynkkpqde.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/goxkdmxat.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwzcgrkwx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gcddcqpwd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gzahwzczt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/ghbdwzzys.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/grhrmzzit.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gkxhlppcl.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gcucmfrpu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gjhmbvena.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gsikrttwl.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gtdryvixh.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gvgpemryy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/ggvafekpg.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gnrgsnlno.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/ghsuxlsjq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gzfhakgss.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gqqdqnnud.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/ghytzbvee.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gbjdnofpt.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ggvyootpl.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gmncedibi.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/grdenlxzg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/grgzvrhey.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/ghclgrgkl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gpapftmqu.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gujdtnami.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gcespdqbs.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/grokhrlxt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcjtrzfvf.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/glfvgmrrp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gwedkvpyh.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gtgpramyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gcugaxlyy.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gokvjxcyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gsmvkjvpx.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gnzezhcev.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/glnbbwdkk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gcguedads.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gztmfwyrx.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gufdachzt.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gnqlbmngp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gdejhljfs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gobeqfpfy.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gstkgwnnn.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gxmkolort.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gjjmssftq.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gkipiecpi.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gttykrvdv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gwufaiagn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gzsgdlxzp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gkhatufkw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gjrxzrsut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gtokpgzpq.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/goyiwaliv.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gjngsxxcd.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gvcvgguni.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gzatepvdw.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gtepntiqo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gwhnpdldz.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gamnfktvs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gniksxgua.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gopgwtyit.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gybujwvnw.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gvlywnxvx.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gapigzslp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gfodfonzd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gxqqyhqeg.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/grubfoyfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grxallzdc.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/ghcprcerj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gewjiicfg.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gjuvwxwjf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gdhhgkzze.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gguyrrxod.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gblreaenw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gjvtxwegk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwgnwfqox.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gaspxiong.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gwugwslqs.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/grtszugvn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggfgsedds.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/guhmarqwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gejtlqriw.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gskhoaxfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gijkywbbh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gwczjeoqa.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gbakpoznh.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gwtnprrbp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ghnrgbfwd.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/ghproaidw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjaiizgfg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gyxtdyemu.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/ghdwtisyq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghcohcifc.sHtML


<!-- 参考信息 -->