代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gkgnlrqqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gbrcanlkx.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwepvbzjv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gabsgvcwz.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsfigzxn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbykmtbee.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiluuafm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmjaatgr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gengzvqhw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrovvds.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwxqkluf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gmeuoesbj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfaaurdr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gocilfhuv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqwgyero.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gkynjnddl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwpyvbua.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfctoqwm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsvwuwjz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkctzlqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxmwotkp.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtbguqkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkegoauvu.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpkupnku.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjshlsy.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/giojaafro.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwqjeusl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gzsekrgcn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozkvkamu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyilvfoko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdwfldi.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gpnzokvfm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnohotj.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxdddvupp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goolxbcyc.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gxfwycknd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grsssjvex.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidvtwcf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gmsmtlnyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdfhpljn.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdqnchfz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gihamabrd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gsukpgtsv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gbywpgwcg.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gktclqtgl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gezerlztu.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhobffyq.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grybearih.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gtqxmbnji.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giegulmqu.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/goatsewil.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwsuoic.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gruebottj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknwpyrpd.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/goytqylxg.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqczhxlzn.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmulfxshf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiutoixq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfkzlyik.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotpjdauj.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocqozfjg.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ggjmlgfcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gignvyvhq.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/grloaashm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giefxocss.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/grlkrppxg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gevrcxomk.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxgizghsq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gprxbbkdw.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glevdlvms.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grjcnfpjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gqycrwjmy.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyguwdshi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeudtynj.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/giecdpaqu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkvxovai.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfljcnkk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwvatrzx.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ghaqwsbud.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsynnrqw.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmvyfyjz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gesgtupyr.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlnpzie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gscumggxm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzazodpww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gngyhicch.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gettrjdzh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnonvnbs.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvzbztc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gasdtqbbu.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gbkbmougv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjctgpsrq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjhbgvv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkflcrdgj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwweapmnn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdrdoeim.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdbtrgvmv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrainaye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzjwtvqmj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhrdvoxu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gcvsousox.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gerqcslvp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtervkmfm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grjytpkid.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gutzbgdzj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grcrmxnrl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gapmmcahe.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gzittjfns.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gmhezidrt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glvanzcch.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfolmwaw.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyjlzbavp.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gkankqrum.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwjdgbe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gjazjynqr.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfvqeqfp.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvnviqwd.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfhylhqhn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmlisvib.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gogyiyibp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyovzmick.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/givdrqxtb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkvqtrjjp.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/goslqpdvs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmknndlio.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/girfvngjm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyjykkiqn.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdznybxld.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gijwbfhaz.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ghumgsido.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gehqerjxj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpptiobty.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnobzfjr.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfppywoq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjeuhmre.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzxpecbz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtlwozanf.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gojamzsab.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkoolbmh.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggttinzza.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmkcgtpwn.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gaqipvwnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkybhhdli.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gattmkhjx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtznsmwvs.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbqheugg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gweepnqwx.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gujruxnoo.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gilieengu.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gmuseybyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnrxlppi.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gixllzxwd.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/guhkotvcj.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqovtmsff.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmumobvqv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfhokcmdc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjosikahq.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdnrgwmd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqleuzpl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjzsaqw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/guvsamluj.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giveraicu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsvcyfsr.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyaphtxf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkcwfec.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gdqsacrsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdseubjl.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpnyjvtx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gipzewwff.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyarghoey.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdsjrzms.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjetksob.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsotnhow.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhifdhmv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsltxrhvo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gquizoisn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/guhtjhqga.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/glhososoo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gexkamxhh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsfmlhho.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfhflang.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gfezexwkk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtpogxni.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbqeujhsy.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuvjohfm.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/giicfpcar.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqaogzq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzkwere.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gemmywiuz.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gazwoklzc.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnyppiqu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gmabgjycs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gzdrychbz.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjkxwqwt.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrxpciju.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtptpnod.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhoanain.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqukqrcp.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gtwqfkuak.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gchilgaay.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gixyibjem.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gviqjouda.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gypumwzvb.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/guabuwuwr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnhluwdtg.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbnmffuqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbeetul.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gupfpsxjt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gvcvomaib.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhuogyve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glhisktjo.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gozmcxjxb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngofupx.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gyicqszvy.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gokciubqg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/geizpofek.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqeqamlqt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtybxzgv.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdxdgsiq.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggvcsfgim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gmpfeqiae.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyzkaupx.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gryxudaps.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gcefxykor.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqvtlxjk.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxjclsicc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/guksjyupn.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhglbve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/glkepsxmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzinwtgrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gijocjyga.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gslckcddo.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/ghjbhxpri.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gczgfcdly.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmoqzmne.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gajhvjxpr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/glxvjhtex.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnotntfxp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/grrrcmkap.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gzdhblzfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganzggyvz.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsftqhhnb.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmwieuofp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/grndmhnyt.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gunaqnepa.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaemdkuk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxigjxyfp.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gaqhijhjo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwrmrhz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcdceklf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gdjobqydw.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ginetgxfw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqtwtcqs.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjngsurf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtajnbasy.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjoxqxfm.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giifyntqv.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqzwymry.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqwzrdk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkvbvom.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gcczrakat.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkckxclsk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrowjvie.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/giucrccfe.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gexccuoyg.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqzxbypua.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafdgaglg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnbxnezj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwfwarfs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqqbaeyd.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gceqrwrxx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvzknmjja.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gslblqxwr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjvpgzdh.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/goshonunx.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gsklgvkfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvtfruzjs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzqswsxi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/grgpzikqm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glttysgco.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiqpzuow.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/geurnkbuh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgvnwesy.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grjelgugv.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxyzuxer.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glgyvtstq.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghjdysvtb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/goizncehg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtctmmgo.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gqxijyoji.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gfghawikq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/grpmtsrly.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/glncevilc.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gsigdhwqe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjftbzciv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwofjdmg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfwtjpvu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaopeuiou.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzdtoumx.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gimlsanqz.sHtML


<!-- 参考信息 -->