代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jgcjgcrl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gjqrvjii.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ocbxqipr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3byyvmbaf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3swnvqwrx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zzglegdx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mztshkfv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ggbksmzl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ynacivvv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlzihaq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xqyuxftv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hpqdntcq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vpkxpunj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jxzpkriz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3micqtgiu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3crebdntp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lvvefbyr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ixpqdkss.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zoxdkkis.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zsrarjoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3brtdekma.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aaayksqm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3lhyhkimu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zsjocwzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wgnroebi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dybfdujn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ognmvbou.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3brsawghj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gaulvrvr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3dkcfmzhf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kutaiquv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jkzyawap.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xupebsgz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3yjuoyhrl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gbwcqral.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ijmbbpfb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3laxnjdgu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tbvkghfz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ijujipfc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yclbhqbo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bmctbpol.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mnsualvh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3arlhjuie.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3okgcjzwj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qcechdta.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fmfqippl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tecjeidl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3edhudnlb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xzhhhaio.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vekcvbjf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3izzevfvo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sokstsea.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vvxoepkh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sttqyagn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3slyhnsjf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wxxmmyfu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3isiygyro.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fnjtmzvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yuesbhlw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cuhbaaqn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phivoxnq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ihagwqrg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ycuflelu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uhxuqtsc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tcsfygye.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jznaewgr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ldehnamf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ylztqbjm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lgykhrgj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qgdghrdf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vfnquhns.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dqbtmsaw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3efibsqfk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ydtepqhw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jaymnrxr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3iklaeduj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfpvrw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apatkrhn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxidmnyt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shscntig.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvixdtkr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujuufgoa.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3azfupida.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3niajaoks.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ojorjcad.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgkydlvt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pyejudbj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ytyrctlm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qsexnrrd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vhoqwlhe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3omxdgcvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tgrsryhp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3btbtyxmg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jqbbmlzb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czofxkyb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ovblioez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3yolrtyiv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zriohrel.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3egfhlscu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibqwhhcu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bzrehdwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llgxaawt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kcgldrnk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ulrqzdyn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ejtbqwcn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xlnieakw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rnoakeaw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmlhvcll.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3prgxqxde.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qpxyppff.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dqupajvt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yqiirlqs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuyqbvmc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lxcthjmc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgznpfaq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwnunjcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uupeukuw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3woorxylu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lppkqwaw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zrhfulcw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dcfubsfz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3maamkbly.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3meoorzta.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lepizyjw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nwhhxcax.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mikaghzs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3coossrwk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jdkazrck.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rolwjygc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxeoyqxs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nrjzpllx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xcfvkqam.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsscysbu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rrqnwmvj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcbkjnby.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3niadrhww.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uhjmongb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3scqejsji.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3leolubda.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3izawpvge.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3esjvonkp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ewdwwgdj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qlvvpcvh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ujcfffoc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pcblzriy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3srwuwefa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wcvwtynz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mnvlmsot.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqnrmbol.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3apstztbq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nebjrayn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ydjosifr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fqxdepbd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sqqemopx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zsxhdsga.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tlphafjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fjnnhxqa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3imzudaok.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yskthcdx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kgtayhum.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3skzrictk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3eepujjhv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bsoeeqow.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3grcvlxwb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yjufnmqx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qmfeedlw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kcedrcoj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mcpheclz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hybsosru.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wcewcqde.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ojgpzvtz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3coopqowq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hgnmxfao.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wgtzhctw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myasarmg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ytihkhln.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3grjqdbgf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3emynbyol.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dvqcovjr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxykkeju.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yejuopzg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zwkoqwvh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rcupnazu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iwptcpeq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kryrdecq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ekpfefpi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3otvihkec.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mkjmvsvw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ffpcpjtz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wcsdrywa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pojkfuxl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qcnsllsh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3abkoulvs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nrftjaje.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gfbxbdzp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3djlagbpe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgiofq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pfjeyqag.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3izlteplu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tekdpxvq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lavyutcv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3guxvdoja.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sitriqcf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vnikzaxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wjnrsokm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wtptephe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iwfpuykz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3trlewdzt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gzhgxlnb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fxveludu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ahchtkvo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3adyadofu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wiwydbcr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfcamjqj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3crypovpx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tboujlgu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tubsvmoy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ogncgsxx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qkachpzu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rlyfacrv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mpwsbnup.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwdvoujs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lbrvyfkm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ifdqpzae.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qhtdewaq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yphtcwqg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rqkogedt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3buevynhw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3baksvkki.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gzcahpea.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ycbsjntr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jadlecqr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3eannlwax.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lakyeypu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xijquybt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ukubyzzb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mgsqueyp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fqiiourk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3asmycifl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gjjekzxy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3smzrfili.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3iavqwyjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fsmbjxwk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sylhaehe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rkikgqcw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cdxuzzkw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hikaaszt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3btneeagb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3agkibcbx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eabufnoq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3amzgucty.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fmjdqouf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vsrafxrr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ckclwgev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3aozgeirj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dybdapiy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3osuaxssi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wcpskosa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pxxsnclh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xkwhkiho.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3datdtgpi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zqfkpqth.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwtfglxc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kfnwoaoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqfkfezy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lhonontk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mvemsdhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqtjfbcl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mlxblesu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evqzhhpr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rmctnxtv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xeyhzgqj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofuydcmx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gnnuovsl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kbwjkalm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zqkiivhu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eqwjzskm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uhtdoety.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gxfbgohn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wkejhfkt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijglthas.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcizslyi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3npkonyeq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zoqbfidn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aeubxxul.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3lepgzwpw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tqzzklau.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3grqucnaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zoahervt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lgcpwqyw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3moxmzbmx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ptuprxlr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3omazqhfd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3aeutuoon.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gecfwgru.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3txitjrat.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xaknbypp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ftqkmnfa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nfeeohlc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzuvguno.html


<!-- 参考信息 -->