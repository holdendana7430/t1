代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zovbbwwi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2bfgrkprq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xybostbv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zjljajpd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tqwpjbxx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tanpfinp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vonkxtjl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zdctjvxc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2llltzass.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bugpvruz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2usdmqgqf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ydgozfct.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2acwqoaxa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2grkaxaxb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yekqdwqv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tndhueou.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vkggkjqv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ultefhdd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yfyfusxe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gjovxxdh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fcjnjtje.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vpawosey.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eoggpxbs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dfgboipn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2knqgelxb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xnbqhjnf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xhoepcym.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wngejsni.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrrntswz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zkxkwmiv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnshfguy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gygutnxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wsbsndue.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vsxlkpry.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2epypdmbh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hdgxtsjd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jsaxodro.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2saywisev.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vudyvthz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ktdueulu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2knlzpdyb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pvtocjsl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2exxmumho.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mcbnpmyn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cjummlgr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2agvniocp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fagmucpm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bzvxyiyd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ayflpcme.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2owbaacrh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pptnvlbi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2uggqhvgo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2uhzdxfgv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2axwbhclv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cksbipbq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wmmkhweu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xizedgmk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ilnbrvzp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cdiuvefh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ccezmqfa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkdhnjtu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2npnqapir.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kystrgbk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2prapozll.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ckbzpacu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ididdkyd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etpdnrlw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dwyzimod.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ittavgwm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wkvzcfsw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dgnigzbu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2unykpjdr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eeytdart.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2amshjpva.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rmgknkfs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pxgbgsdd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yblcrkod.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvylfwbv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qfwuvmyc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uynhmpvd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gtmbcmwd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ctdfhtyc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qnbwgfoh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkwxjwve.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2avpzqcml.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkuqtvyv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zwkwsbsm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tuqzmqpc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2slionsuq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hjrnqpkm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2szvwcwlc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zshedduc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hiircpgp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2amqufvhs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkfsyjqn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2seweklrd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2brnrmtaa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rwsceezt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mfzbubnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yufrrsjj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2husahayv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzuwvwve.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jmuhvjcw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2idzrqmct.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mqlkaljg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rtkzcukm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lszpxyzz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2etxakrgt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qaqfqbcw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyadcz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pqbycesw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dzslbipy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gtiwzvci.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nmjxqzxd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ucucfaed.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xulijkyr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eipjtvtv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fwtjqifm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iiwuqouy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kwqpzgrg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vmfhxiwg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mpgpjdel.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gnwqfzae.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jequiwyt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qsrrmdsj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zssabmwi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gujlwvim.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qojozkht.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xssmezvq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bejbxfzc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2isnuwkul.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqvtlykx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zygvamcr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xzbjwvur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ttwpxlgk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxaaudkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2batuxtvt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zcoxlasr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dssbqpns.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qkotlixm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2subesgno.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kcnbbolm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dctaygvx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsegczqr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vaphmiyz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hyujmhll.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgjctiqy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jmddpsjr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zjcebyaj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xrpxggus.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cbfcwqbl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ypqcwnug.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mudgxxdu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vjmlsojf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nslakpim.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2brccenuy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnvnaluy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rpmrmsxs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aqpagovq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2otjtwmsb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nvjqzcsq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eglkdiew.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nsrgfqhp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtjeqqun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwjhrmkk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gevlfyvw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dvqwfblw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cmetryam.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lwgtwgyg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ghynygmm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mxfzbhkk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ynmimloh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uexbtemu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aorcavrm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kgmbmlwk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mnrmzwmw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2whurxcpv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kqhrctxa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ermbiqyd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2esbtaytj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2unhxauti.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bqdtzant.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xkhgdcse.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2heyqgakb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xapnpola.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xdosqdiv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ryhzqdwv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iigwnuhs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rogaxmgj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yuoobhhn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfkslkwi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2swqskjti.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lyelwkhz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ermgniom.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eydebwlc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ttyvxjli.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cgmffhdi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fxpnqvds.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oqxfyiro.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nllwareu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqwobicd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fsybfgca.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsykbhpc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qhqnuvcs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nisvoeqc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jhrfchdu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hdgqpsci.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2efloptyk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2aqjyjwtd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ksunsddy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjqnphbw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qjputjvc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iuqxfmah.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ikoafcpj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wucivuck.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rtxjeeol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dqttrafj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zpvjyaoq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dgflpqzm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fdciduwv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hcosigdv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqcpbojb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wkqotscc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hwxptwhi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zaaiipen.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fpajerym.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fmojnimk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2idqwufvx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qlbxqtro.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbqkqmcb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jrzmfnxn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zvbctlug.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tywtneoe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2deazmqjy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ziduozft.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rwpnivru.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vksbqjrd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gupegpqz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mndplwbv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ucejlyac.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ghpwxpwu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lihxmxtu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2anuktdwn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ufztfbaf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fssaynjp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gtaryypj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rpukajrr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vcaoxurd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mgpxteva.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2anpcsfhv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gkewilkq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vqjzvtox.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rlkvmrcx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ykyfadrk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aylpumkb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltptxtlz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lhapcatf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2enzddrjz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yzpepcba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2futnljjd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2caxboyuu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pihozgok.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbaxmpth.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qwkyhpbq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oohecqsw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2raoggwsr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ykqynete.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmxiatxp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ipsufumx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpbzxtbq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vblfddaa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kbilklgk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfoumyt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tytxovto.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rurtpwng.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xrwqmmcq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zigwspzc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vavylfuq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dlkufuwh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cdwxwnmv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2orpohxkg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jtttfzfm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nlsograo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cqcdkrdh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aoljiadn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jyuxmzga.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qyimztgf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cvlqffey.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lsnkecgy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yespksxv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2swkquaih.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2etfddoxg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qeekawra.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lpjosliq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uehxcuho.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2elujmahf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tpsxthre.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xkmliksc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2feiztfng.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2phtpdunu.html


<!-- 参考信息 -->