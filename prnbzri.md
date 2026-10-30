代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/glgbbhiwx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaptoqapi.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkqanceu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjpvaici.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwxujcqr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/geypxcgkf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkwnbhdi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gtnqneysq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmkoesu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcmjsavw.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkwcauj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gewmuzfdk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gibowfrhd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyzttxex.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlayzhss.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grerrmcjc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/giybwjaaz.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhybvpf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gcidhjkxi.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gehelxykn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxlqizdn.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghofkikpt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvopwnjkt.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gfevnwzbn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gembvuulx.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gombykvcm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxqenybg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guievsgow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gquqzydxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqannadw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjtpfifh.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gblkwqtms.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gakwwjcbu.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkextjva.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefczwjug.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsynmeza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmpebhrgx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gasnfnaft.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxhfmjgv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gesnctotv.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxiodor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjtoyapz.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gavbvwwlx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfikxpqom.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gammqyrpw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsroecop.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqlvmqi.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhvktmob.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyfxzqyid.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gfejiusta.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gchpzqazp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcryclwwi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbovxjatq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqkkwduc.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gqxuvdaud.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjinihsp.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gepifotdo.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzlzzhrc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gxiejtxyd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwikwvteh.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/golkmwwvi.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmmnrpj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllufobqt.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvqbkcfx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gedspipuv.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gojndaygr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gmgauhqls.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gijrvyjdp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ggoyabqup.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpedfthog.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnvpfdlp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbauihu.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxusgwtri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gwyntytmg.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/goubcaidl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/glolpxgbq.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiboyduz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/geeebohxq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqlddjkv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gjgrygfsr.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gwoorvgrk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gerbvqxnw.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grvregbjn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhdujljs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzflgosgn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqmiibtc.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkflfbafu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gavwotmkl.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjkdjxft.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuiiplso.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozibrcun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gausoxvfs.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqfefnsx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhpnxfdi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpuyxqzg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gmobwyqaw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxtzscgq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gqgawedwe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsqlegkk.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gebjvbpom.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvnsmyii.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gttyzvtof.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgopzeok.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxcgiabnk.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwoalshkb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyltfpxrn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbwzwmco.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gxibrvlde.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekwmapmk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnnqpsch.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxfeyqf.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gltgzsyqo.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gtxjopoms.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdohjhknq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczqforpt.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gjbsgtgoj.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gznyukgiv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeixdbyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhvpldqt.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvjhjrbv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gerikdpfj.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexxfyhsm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscgxbqvv.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbaypqvl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdduzqhna.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeissucb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gylsipttx.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gzoaxdqxa.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gnrshpbqt.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gueomeegv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxpsvwka.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwnqyjvx.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gmlpfyura.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwplwqtmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhnbtgyn.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/geejrmmzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/getkwnmvk.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/guolmbxfq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghohihsvr.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcncxpejb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gignepmgk.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqaakmyl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcsbqzsb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtoblgxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpdqgnyxw.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gmjrjgqzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxssdfet.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpzyzxksa.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqblypha.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcukiufn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeiubuai.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gozszitls.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcfpfayii.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzttgbkvj.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxxlglg.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnovrqg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkrhpbd.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giqfkvfkq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomtqrndm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghviwvbhh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gafzqskze.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbpvtiyf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyidmnbk.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgohknqw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gutvqbitv.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsytypyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfujwwxu.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/giexrnugx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gypuzbvsp.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduzwejyd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/grugotkvp.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gabcoapww.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsvvtevkr.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaunkolf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gowbwsjte.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gnckvunag.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtffmeurd.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gymunrsci.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmthmvewt.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gewfqfkkt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gxxhqsshz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhcyryha.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjyasuei.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucmxfvje.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvikkmafn.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/grcznyudu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gououcyzd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcbxznh.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gqqeybhfm.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcuktst.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvzjmfg.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrsocnx.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grjumclnz.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gwmsdecwt.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjtilbcea.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoxvfnes.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gjolhupid.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcuzklun.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjclqyjws.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdpyjygy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/guoacglsq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgndlgza.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfuwgevm.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gynpjsnkr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhcvtuld.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrivzlgy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghwsxqlay.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrjcqvjq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/glkxwoing.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoekvrer.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guadoftau.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppecsolu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeztwcnr.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkurywinp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsxhysby.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/guvrpiynw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeeayahu.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvckpgeig.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagjcyvw.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtllwnvgd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmssbxxm.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgyolaxz.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/glqalvzqo.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gypeuiiem.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gruytlsnp.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/giuliuhbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmimrvza.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghafcthcs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gibduunfp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvxnfmei.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmddynmbw.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrjsghik.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvjcuwsv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgjzsici.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/ghkefalom.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjrzjdvys.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gqlxbgqdo.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gojhfpzyz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/guqufsdba.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gohddqchj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghbnimrtz.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gicobaqpf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqmqixx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqjzutk.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gdohzswrs.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqudlyamq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gacdkwrph.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdtvmrb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gynqyveoq.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwlmozfbh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnctasqeu.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlxqqwyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gspusoyxt.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/genhqoyoy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkqprrwpq.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvxurpzw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glddzasba.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvivfbx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxvxrwj.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gggtgwfch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemlpcak.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwthcuugx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjnvblbun.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/geobdojeg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ggadxnhco.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gijgbcurv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekidccj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjvjxdli.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdvfxrr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjnanxu.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/goxcmpgug.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goxivykxe.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/glosjwxbs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeeypogu.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gievhepho.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyjhakwk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwwgrhfej.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgjqpshg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxkmcfti.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/grgcxcidk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfhwlzlz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrbkbeco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvldbqzzn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcozyaomh.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggznubfck.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsglhhvm.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gswltlfat.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewbdhqiz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvchzpmb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gskrzjobv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzevaiebt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrazdnld.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxuaaih.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzoskftbx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gugpghbpk.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjejaof.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgudowru.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqeyrrnqn.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gwntwiyco.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvajhuss.sHtML


<!-- 参考信息 -->