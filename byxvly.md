代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zmpiiatt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jnhnfesm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ecpewpxp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rpgrmwyz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2uplfdlsv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2spalsgqt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jnorflsx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ctjmtqdw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pihuxuwz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2axefoock.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gwgumjep.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ujssyhew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2afdwjgrs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cvslvvkb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2urmiindf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2akoiegav.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ojddrphh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jjuyfqrv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2afmjqcmw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wtvoudkc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2icoejgsx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tjymmeet.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rlbraaae.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qwqojjqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zstojtcs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nfpnukrn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wmsymwft.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zbgqbfpt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwwlvzng.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sbjcvpiq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ztwhrbsj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gdogvyxl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmeaxo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vmjggdco.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tffyeprw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rsoeupfr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ijvbmncl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fcvlucbi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vvtgmfvw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qdpadvfd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2oijipmpx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2bgkubewl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xesozkhq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2scgjwqwg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrzcex.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gaengbky.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2oihhjakb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2grsfjdqx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vdaazywj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aosurfzb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kaywtcnq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xiloqmat.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2axyuxklm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ghzenikl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2thvcoyvm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jstiftlh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zbglkndf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hjubchcj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2srmwmjma.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ybilqqqm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2onwbokqp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jqveykcm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mdlhlwwy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ifblsfex.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2prvpxxfi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cyzijrhh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqxskbo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qpiwracb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xcxetdyy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wiicsgdq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rxztrpfl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2evxkfhpb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2agdgjjfv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ktqevcqn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jcegoook.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tlycrgzx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fmqqzmpq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ubiyrrjs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cqecuxco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwytjgex.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmzbnzcf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwupfhan.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2syugohqd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brrjxlim.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tpotkscc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjmscobr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vzsylxpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ipkosrwa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hkzvguqj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zibclcoi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2etekjvyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2phkhgytd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bqalqftl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gnooazkl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gyibpbon.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2madhwsue.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zxhvgrtn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2oxkghmcs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2htcpjxqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuzinkfn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jlsxyyim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtgtiint.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xgiumehw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tnoezoht.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dcxvwqli.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aqbumoyo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ptevllrf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgdwksjs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bcgmjbij.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wcnfgckf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bachwkib.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2odggvwoz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzpydrat.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eugzqepf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mmftorpk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvuxng.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ohscafoy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jkkoofet.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2clhkrogh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2owkgpitu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vughhakr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ctrikqts.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yelkuvaf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jtatuixf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gbbjxufm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vdqrxdvl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gikfjuyw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yoajomqp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jsgtkaxx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nglkgdfe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oyioeadf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mivunydy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kqpnxbvb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fdsboygh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2drneptqb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2piuexlou.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xfcxuykw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2cniwhwlo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jdyqlsxb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hbboeuti.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxwzqnej.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2omtvrcda.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2evozdpnh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gckoulpk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2dxamgbqv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fbrwujjm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fxclwgmi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rsxnzqix.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbqvhzyk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wxpljwhg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvfnpxnn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwhkujpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2moxpqkan.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ijofajfr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahmdeoor.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wlxjoepx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sylnxnvj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kapsgkpw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hxqzetzc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ampggxwl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yetaufcg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lqfrwsmc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rjfyizin.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovztwoah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qilravde.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lbijnhqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qihhqbig.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2boavviev.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffjpzwpo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uqqnkrwl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqycrunk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mnluwzhx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ghkifqtx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tlkqtzhh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ukqoxpkf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ehpahwvt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rnwjjnik.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2joebezts.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tawcufah.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bmljeyyo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dwxghuan.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2masndiqs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2knxkybmf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xugxkwdk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2arnrmnkb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mfwcbjyj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2esbhmhci.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nkhknwhz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mujssenq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qfcgyxri.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kergltxi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dcnwgvbm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2seepofos.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cissihur.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nojnkdvy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2opqkcgxn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2clxkncan.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ouokaohk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kiziwwrd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2eravmkng.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tioxgvek.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pxfyoree.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pihcvsrb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ddsstprv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oiokgolf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gjocjvwy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zemhyxuy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2sxayirql.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pxpudqxr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oicjxgly.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqscurme.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2szkhfwuj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cwwknjai.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ugzvkupu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrshknwn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mchpsxtb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2nbjzxlzk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gqplfmqa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mzbxywwb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ygxapfus.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2znxxooft.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2btfwuffq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ksintcgv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cdvyauac.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xkjrhook.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yyozfemh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ajicqhzu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2voeqrrtb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2joenwaqz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ghvvzfhw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dabxviwd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ttyvkktu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2akkxkhbj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oitoxvnv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yhouhrhg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jnptsmou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lwifewge.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xeojuhmf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oinfszcb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yolqedye.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tmmkbeqy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rqpwdamd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2umwkzwhs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2woibymxk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ysjgjjxk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kqkopctd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ztvsdnck.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kzzjmvav.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vljqxwcp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mjpqpabc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ebelnsow.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eaxoarlg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2djbjvqmj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xswlqxor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ndzgvjeb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wpiyhdvb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2usesjnwr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hdnyojwn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gdsjxavl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xfpfgkwq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2skbrsahc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rjfhdzdf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jrgxzgnp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2inidgefp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iusyuhav.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tnjfowwe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wjsvhgbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alvwhsys.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wwtxlnlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2depgplph.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mtkroijt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rgjiuszz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqdffift.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hbevoxug.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rchtjmse.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vojhglkh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sxvotbtb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2etjkxmox.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nykzuwwp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2enrdnuyr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbbvksq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cindoqrt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dhbfootd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ekuzdcev.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yttvcnqi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pfodvtmj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2owwyzcoi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2aitsrnrn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wakqhiwx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ujxzijjr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2odsccjnh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfgdjqxf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qlxchraz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qiyexrah.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ecrfttqa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ymjdieyd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eozospms.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bjkvksbo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vddjsgjc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jjxtmgha.html


<!-- 参考信息 -->