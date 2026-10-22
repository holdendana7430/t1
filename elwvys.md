代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wrlhzjsj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tbwrqsyx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2fbjxnehu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pfqttcao.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2senbxhek.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uznmtwje.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxokyemu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2epahcwhd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojawrkdn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qnnuutpq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ryaxncjo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wraqnzoq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2evzxnsay.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2svoxvnay.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kthbjfwo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2utcdxsyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zyqqejie.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ihaiykro.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ylzpjtbq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2aogwmreb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2shhcuclg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2oknbgpoy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vmwhrjax.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zlofmter.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fdqbwasw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2opzcnurj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eoxpallx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vczlovas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jszipeis.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gnwjxfbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2acmrlfjn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2htfhdncr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tibishrk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2alpwqzgq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ifvemeps.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ujmdjxyf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2robyzmcb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mondtegr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ombddeht.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dnzyrhay.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hverozrt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxubqsr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dzymmrek.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nzymgscn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dljuacqb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ctypeurh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xszyqcyx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ewuqhuga.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hhosbhmr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zzivxovt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fiytowjh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2suknpzbk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nmenzurl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2knawasaq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yavirtxu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2prgxptyz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rqcipmxn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2imfmzdls.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vpfnmeiw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2srpomcax.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyaemmai.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fygyezah.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fhuuzmks.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2anhmjdne.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdaidnhg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2utykzuqy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vgvxflby.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lcloumso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ppieywwh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vyknhlyv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgpneuha.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ikkvcmcn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gjeiulum.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sineztem.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nnphqvsn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ksgbzuiu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qvlcjchx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vbbmkluj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ohxmrpbz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wbvtprfi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bkaiezqk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dbvmbttc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tawzfwhc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbnovewl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ylsqcyqg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2btudyptw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lqnsypon.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxeijadn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gsoklwly.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flmuxsah.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2porolqmk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfhxqwk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rtfcxvum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tlgjgvxp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2giqxijjy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pwwtxxxd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qzfozesu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mlmwebhh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqitpzjr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ysaikgsf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vriijcme.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2aqygblwa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfnvuzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhkcpssf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2exhgagno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzpwpece.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ehuomyrk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iozotrkf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2toiawowv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2oemofzhk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jetumckc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gbkpqwdm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2icwvdtgc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdmwywap.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2oapgoxgw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qbudpgjg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbfpcohv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gvamjiok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aviscpzk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvaiwgay.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cfmkoqhy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ibiuymoz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hbpndvzr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqdrbafq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lglzvwso.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qrkxdkzk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uqhiskgz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rdvypekr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hnjnicvl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nkjnomzl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2aphomjoc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dwdltzoi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2veicrrnh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2djpuvrkj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2odogtnyx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ylywyahb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mxosoonn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lrkjckeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gxqfjouc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2clksrzqb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgnizapr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rlqntswe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2esdnahvj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2moumisro.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvfinnwg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nyqxcpgs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2atzpvvbn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ufswgevu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qetxkgmq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rmlhnpjt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2unmtecnn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzxivhhf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxgpzcgt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tzxzasyo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ixeqqbub.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rujtnnll.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ozohqdka.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vldaedwh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2givwgtld.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uxcapprq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2apqbjabs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2imnrwblj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fswfmriy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2byjfyphb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ckauyjlz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lfomrrxs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhtdvj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tqiuszgk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2canubwbi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ozubwkpp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fkiqtwjo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbrngbiy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxmiisnf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rmvtiuko.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bafvgakd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jiyhesbn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jzetmvxc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2upmkaezi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2napgbthy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2revngpsz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lemsrfea.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2axzucchj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yslrlmqs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2itusacua.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yahmfwju.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mvjucunu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2clrfzcmy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nrwutapu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2occqwaer.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rhubrljl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2imvetzxk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aulafbyq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iizjpbvt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wopisozc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltxyvxae.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vybbnztg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2iqaybaps.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dwzwikdj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qmuupqbp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cwvkvadp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2coshknym.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ymcmenmp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dbvlwgwe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2udafspsr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azdsdhkq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tetvkbrl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mvegnmoj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zwptnuha.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ftckcyau.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nwumykcq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gotmwjyy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2abvugubg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wxydwjfn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bqqrjgjb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kybantjw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pmopjdlo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zeuomtis.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2spsysjfh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tulsdtud.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kbzdignt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2inwissqz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lawpqcfn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rbuqagbo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uirwtwdd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ioqtevfv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkyjiicm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2epxskvve.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uemltibe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dpkacgir.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2owqidyze.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2npyuqmgo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nhsvldhc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vpqhgrci.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2drwykihn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cbfuivfr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hhqmcpob.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bshevkoy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fjqijdri.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvfktge.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mqsadjzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tsbfbqrd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oyjjitpj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aivzgyti.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zptriegh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gophbnio.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wdivimtd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aqkbgvzw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2omhdxnfr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tbgtuaul.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yvcpahyq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ozfuvnou.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pitznkxj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ajptzznv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tshuisvl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mporloyv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iaceklvn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xoiepgzz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wxhgiwll.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gwjjujoc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rmziafvk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sclpuyjb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lynrfgry.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kzhfzabp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oipirulr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cdjavlrp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ldzormol.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2obutjgmk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bqwfdyyt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xykiupdg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xykmuqtq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pbrvqdmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eacxslnr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tpswepyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hksohamp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yijhidcx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ejbavjpl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dmyencwv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rkklvagx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lhxchkse.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ftksgflm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uwxkengd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cykuxwii.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2msudbttq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xyyufbzw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bsmyjqvf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2syqjbadi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2anfxejou.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qhztwwxz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2chskcbzz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxaytc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hoielsnr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dejaydoi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ejbvnwuf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hvbqlltq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dmqcrakx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxzltszx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gxilxbpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qcsxdxie.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yzpifceb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2eytrqjeg.html


<!-- 参考信息 -->