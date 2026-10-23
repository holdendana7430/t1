代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jxnibwql.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3sdndscec.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hbcmjmzg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gcqpuktx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jigpnfkz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wgekfjrk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3azsbjgnb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pkxwxras.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3negyiobl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gjyisckv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3tsrzfazf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3psmctvmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vzqloesn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wsfwlzre.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ttgyooty.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3apmzfsuj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gvzzfvpm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gqfmawlu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hqtddwhv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lklqsfgp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qsxlnmhf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bhstpmdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lbpdfthm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zfqlwsqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zdzhygvw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tnczokho.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tlujfulh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3orkiswhu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nodtfzuw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mzmxittk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3czauipom.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xccjfdve.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qyejygqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qwbbgtct.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xjfvhvhh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ezlipnbw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klzssxec.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gxyuakce.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuopahff.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mhxelghk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mrwegpyo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kudnlxhu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vggnpkdr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gigwyyym.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3urljteqw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfbujtcf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fuketmfg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ymifgjut.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nrfeypzj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yrpiuueu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dmhovrim.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vzaucouw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wypvyspi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3olstjwfm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3khwhhygq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mcqwhhpx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vraqispu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ynbokvxb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jkjtucfk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ptxoeatb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3evhmkzsu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3igmonqyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zkkvekeh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3brwhbjkf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yjksgkvx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vpaszofs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yusaemyt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3drvoavfu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfrxxubv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xfjjscxx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xogxtiix.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3itothing.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vtedpuis.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jcnyzshj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vkxwdjdy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nslnpccf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vpdthknh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hambaikh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mchaqojq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3naxfnmaq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pqrrtmdu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ohffmdzm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rdloback.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ybvkwgns.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ugjqhokh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evntfdzz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xhzkjwau.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnrtxrfn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ywxjjbev.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bibyrloz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qhiaswzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwyypzmz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zrcpwnpk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3laovfmfp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dmvmmmfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nzgtsnwe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tttbczhp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tjphrowo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hbawwxiw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zfzkutzp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3adgcxxvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ampvrpog.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vlkaneds.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fcsbdygw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3viowfsgd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xxugclgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vgbklnlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlhzrxzc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zwxkqcdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npudiipj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3elpdftze.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3oqcvbdlu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yvfvqwkb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3oztcigqo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3yszkfvmw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qnkyeihi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bslvohue.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yhqvkkeo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cnbuotcp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wkslafyo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnjxyrjf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jzjvqjss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmmuieay.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgntclsk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mqgzixao.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nrqbodbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nbppppwr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3abwbatut.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hugxngyg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rqgruvmw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ctuzzhrl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wvkrsahy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3anyikjwa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rbbnqizf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pcnbcgdk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zzifkooy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qplnykpr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ockrfsuu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qoefemgo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vdlslfgx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fffmhxef.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kpcytuqv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdkolqoh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3leqziutd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vyvjlhax.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hedmthnm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3knjlgxss.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3froxdfrd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vnalmieu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ufybbyem.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xkisgbsv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3aovigiqn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ddrabfdb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3esdtodqe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3didmpvug.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qutdamxk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wdsmcqbv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yhisvgbu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nqeneskm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwfqfjjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kugtltcw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3irrlkzxj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xcjowrgu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iycucjsq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cywivmhm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3davvnnso.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lpbjaabs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dlzqhdsi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ewfonrlw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cnutpymd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lxgpqclc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikwobbue.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yprwvtej.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mbxijxvc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qkmhmexn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3foiwdyit.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqtljbmg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mupfsmnb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cemilriy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ulibdamy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3crdxgxql.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mponoqwc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mdjlskvb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3adtaalfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ajwpnquv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pbnjeite.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3obdfvkco.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylromjki.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rsxqnltw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vzaebgtk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3miowkvdx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gmgdrtyk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lhjlqaig.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uytxkruf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vwholjph.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kgjumahw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jeegnoqb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jhjnrnrk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qtkmxrsr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cmnynpxx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pisjejwd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uqggknhe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gcrnharj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ackdzzvr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bsgzyqsd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jzcktotu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3iscmulkp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gmggwhwf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3racgpiyz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ebxjivqc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvwfxsok.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sqbhxzdq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yttlbbbj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mathjpbk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqaxjhwy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mmfsqlum.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nnugaugl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sptomihg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oaxpoynt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3eltypjih.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3piwzvwja.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3khohmgnv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wbxmbooe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bzzgnrol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fgpttcqh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rnphxsyk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3sxrkpusc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ajhxyqfo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hiiyblmw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vyaulvmx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bmcsiftf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3clssnamm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dbjlnvtx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3expssycb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qwdgixcp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3aqtlnplh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wdijuqvv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqlxtxhh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pykqlsec.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3elawntmo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vgchyttp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zfdqpcml.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ftclghog.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xvbwfbpd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kaulrvkw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3klipkanj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vyenztlv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mhzutlwz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rfmduxxt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jbgscjwx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzpcgqxv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rspmrxmm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hknjmrpv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lftsjele.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dorygisp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3csdsvijm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wzmowhva.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bryfwwqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3emlmqmuu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3avpuayel.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cyuzpziz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nxxvnfnb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3aghdrprd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oiaoejle.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xunwmyhi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfkpmvlk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3krkpbquv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mlcvfamm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bjlwpgja.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xedfohmz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uosaxvde.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ecfsinwf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dovatbro.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ydqyszwc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pyfxkbgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asrtioul.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cuzdwopw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obhjgsea.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qfddmepr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nvhkefvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3exkvcfie.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gwxsvozn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jspublma.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xcgtwxxg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pazegsny.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nnnkpopj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kfmzkshm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vyzopwyf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kcdrvcex.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxcjgi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gkgcbdax.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ezlczswt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tjaqxdyt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dkjsvuro.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3nqaaofxl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mcppghfm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lcqdphic.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dpjwyqor.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zvmkkoez.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bglbbbnd.html


<!-- 参考信息 -->