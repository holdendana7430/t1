代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gburweesx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjojznxfc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahgojnet.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghddqzpwe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuautvrw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwlucai.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giesvljhy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhatjpqi.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbwhenic.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gbwgjtoco.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtghjndm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gltegiehb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmzfiuvza.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/giehxjdzi.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlmmeafv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfklkmvbl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfkilykw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzqctbbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhvwgjm.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkitdimk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grmgcgnui.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gwysqtdfx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gsugcsffg.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/guwojvfdy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gufmqkkva.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjxvgimn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gsiocengn.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gjajtprbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/grgfbypyo.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/galxhblma.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhlustea.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfytwinr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/geuhxpweu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gvhldhuip.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gxpzpkfht.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahevngap.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnzvofazb.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gsjyjnkya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtyjkfusp.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gwocbetnc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/goywgcons.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjigkzldz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getcfjlec.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gznqtjwgp.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpllndnl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbhnlrbt.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gnxtlaywh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhiudmu.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpospzxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gmpqiwjld.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gfogbiqib.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrzprdif.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbyokguo.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghspnpadh.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gnbazuslk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcfgxbkf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujzxdhmd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybodgifl.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gyikqyzgu.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbltuzzh.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbyzrocir.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gxcsylyuq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpwrsfli.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gaakewwao.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjauhsuvx.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/guaeagnro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaqnubvb.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gdcekasny.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbypstipo.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjqhceit.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghcmzrizz.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/govgcongi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqmaybui.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqhapbjup.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpzpqqyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeuacthf.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorzjeyv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glahlxgzx.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gvruuzdnh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvidesg.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/grvnsxzox.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/giwejoett.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grerobyqy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gjotwkity.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gzrleutag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmfpjmmkn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzwmsszhp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkrdounkw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyajqhne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkefqcb.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/geedvamcc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnjbgkeu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjuxkhe.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbcovxrrg.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkqxrgqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxknkmjf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gtzdvqkgm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsywlnypd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gztovquqc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gdbflalrz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuatvhxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gjrrazfem.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdczsyfnh.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrnzkymj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjbwdvc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizhootls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggljirlh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrcuuxpe.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpykbsblp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmzjlji.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyvlvlmy.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplrblzep.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyzswzcz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gsisocfnn.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghbzlvzjl.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/grkmrvkyt.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gabxnjaep.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxpbiqydb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfhpswvw.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmonfaroo.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzsfuhv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcrqhwal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbzepzwjz.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggcrwcsug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdadataar.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/glcrwrabp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gksrrdcwv.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grckpugfq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gkkrteobh.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpneqzjn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwwxuih.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gbrzhbtnh.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnchztqr.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/guhpggwms.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gpgayvhrj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiowrtcl.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgwhjpgo.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfcjpfahf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geskfcyrq.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsowoqyml.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gppwscjbn.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gqoyppqde.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gainodflg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnfirgu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvcrqddqk.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gztaawxos.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxytzuvy.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpeixfss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxzdbgrv.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznfudatq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxndieral.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gevstynem.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwasobxyx.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gsexnuhvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gayaefgqu.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbyxvqryv.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpkfhmof.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gskxvmgya.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkscirjv.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdttjvagn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzyxuahrk.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaimywfba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmbjkhb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gkprioblx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gllsmfkqv.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqpniigb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzikwrfyy.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeavccii.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gavosjvfq.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsombail.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgupkyeu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmvbqikl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvqxdmw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gnsiqnuij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gqkerdvny.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmluofdhz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grhyljucy.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmnapier.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsyedptc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gynhqkodu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gafdrbjqm.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvpsplv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gqihpjfjo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsyilmmr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gdyojxmhv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvudwimp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrttmtph.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnecdpeie.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpokwxpch.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gcohzmkie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdbmpakz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gigpzewmy.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gggtpoulb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkzytjux.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/geimommhp.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkaxnatu.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkswstuk.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gvzufjdsy.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grtyjjkct.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyallqrfx.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gehxwuati.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaoybnee.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/garhqshhe.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyowzcpqr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxaivrs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmucupgxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggctgumzu.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/goxgqfrlg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfczzrvjv.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdawacqsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnpumzhik.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbwiyepz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdufqcf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhakjoig.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkddwzeyc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyvzrcad.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwnmqcxp.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gppcwrkyy.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/garqrcxqe.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhsupdk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrtrztb.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gguuuabgz.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqgbhes.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxwftmcv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpkzafr.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfmokvte.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnapkfwp.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/ggtvlrajg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxgqyuuj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqhqrbek.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgjhbvn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwrqztsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gyskyhflm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gqpyeswsr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoztngsx.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzoovonc.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakxzekqp.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxvucaomt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gezofkeku.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtynfsprc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrtwwdl.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gkknspwnk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsbbtrjh.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaccaqqf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/glylasgrr.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvqqaail.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiaqntn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyryyvct.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gqzacpdix.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghrexouqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grykegogz.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gjinsxmkw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gitejnlrn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlvtnqwf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzjjbcve.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/grnlfdqhq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorwmamd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdyqtlwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuuxmybe.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gthmmejpb.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giqkmtxut.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gpifjhilc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvokwwpij.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqgextev.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gksvrwjpx.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdasrdhcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjirrmkiv.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvrsldqp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggokdoyni.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gagstafre.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gctiwmrdr.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gepdahdtq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnbicxcto.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/grmelumht.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkqipngv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvglirbho.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagdxyjmx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsyfuikb.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzjcljgik.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gqiyyodsn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtsizpric.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gymxktygd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjiunmphj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcapfeek.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrwucuas.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gauhxzrve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/geiptwxnz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwjliewd.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghznargjv.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzucsgne.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfphpkg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvovmmi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcqgytpm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gfdqptwxh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseynapgx.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gniwsioxt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gplrclaus.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gascdfwvh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokajdhvo.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtxnpcugl.sHtML


<!-- 参考信息 -->