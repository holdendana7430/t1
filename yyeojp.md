代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3injgsded.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oprmccmn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xejgndnc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ozoctdqm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jmbjntfe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qgrlxpes.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wskpepbm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fvzfolnz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zvavrqyk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jxzjmedt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3pzprvofo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3myatccno.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jpcdpyil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qzepgrgo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mctrsfck.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bbzvjjlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pgyovbbr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hpyilfix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yblnzinc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vcmqyujt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdxwksbp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hfaqxexq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nrykbhki.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tleulgbu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gaicpizv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vlqgmfrv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zxwbkzcq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rwivybyn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3atabnjqp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3igebuogo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ryjkmohy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3srstibyh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qydgzryn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3kfqyoufu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kzqvwgct.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mkweiaiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jlzbtzui.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qkwmiltl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3oqavcyxn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cktxznoy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qcgbkqbp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nqulmkjm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vjtamzul.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xogoydbx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3msmleafq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pzxvjlli.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fgiofcfx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yzxlxptn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vdhfdryn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dazkcpwd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jrwvtthb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rzdvhfrt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lutxdebo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ivmrkoam.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xnpqwmqi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3apyihqmz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mylmmwyd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jsojxyxn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wblylpfy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gobkvqlp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xprwpmrq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3eiowoign.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ofligjbh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cvzlalgg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eiafndvm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3uubksiue.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wdzcchyv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ljrumpdl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zqnslotm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qzoxeumb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zpxfpakn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ioyxczcv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hnetirhc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wydppeor.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zbvoypeq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kddwrfxu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fskxecuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rvnyszpg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ualxftbk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qjfoheee.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3acqdfbxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvsxgpvs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkoajczm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecwnmfsk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pjdihioq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldeqjaex.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ydmlusrc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfuvyjgw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pgtfccuw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlxjudjd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bzhtwxqw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3btvuvlob.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fhsijhiv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3crtsdvxk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zczddkhm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3sqrjjtlm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kpfvsfqi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gakuyila.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agmitafp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qjmsutxx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qjwgwoqg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zjbiymhw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bgivzwfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdsisqtj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3scweytyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcybxlby.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gwedlhqo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cvehzhvy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ttcigrqu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3roplptbw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3neyyzabb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwgncdmt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nnaccfsk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvyhvmzt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3sjwegtqa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gcozages.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvgmvvir.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oegmyjnu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rirydctw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yetkhtfk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nfpecnno.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3txkdtfcr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zjcaiyda.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vqlmdpub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rpdipdms.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cqkkkefx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zgsymjxu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jwchwvwl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wgpebhzg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zriqxcsc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mdyevqig.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wmudenlx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qyybdlmb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lqslvdix.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3scavizra.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3puucpxhe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvncrjrl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wbhqzxky.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3erlkpsbj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3flmypbsm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lbhhcxqs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ojylunrb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3slfdtenb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3utgxxrnh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhylegbb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjqurfps.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykljgczw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uputlzfc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zsvgqlgv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xkbknpzs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hixaxdcx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lvcpdobb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3spphvhvp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3knkbtyxx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubjuxmgc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3blbrtdao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zaslodio.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iulzjrvs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hnftvnqe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mvwgwovh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vjtapyoo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xuqphltc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vlybrxin.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3apqzpiyi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3takynmku.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cpgdblvr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rivdoxwh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilgpmxwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pldypfix.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ktuvjzeb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vxnrtxbd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cgegwfsr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3shfywjfg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cysoqnlq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgrbosr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lpkigtwm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dlgoxdkz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dcetxass.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jvcbcznd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kdzdohrs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yakfojsu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3veaeulmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xomjkhtb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ufeyyevu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wvucferd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zxnjbftt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kpxvwzyt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qouwloia.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xfosabfy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wpdlramg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dexvqgww.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3oyjqscih.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sxeywwfs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3oyosgnam.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kpllqqef.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3umfaaaku.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wvzpydwg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cnfygkqy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uuneauep.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kxfnhpdd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ptxkgeyy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zzvwwuzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nfmhufqu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rnyntxym.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3plvfyiqb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ooxsflkc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mabglwuk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ovlndaeg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3otbveldt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ncekbwkb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxfaysxu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3decoolid.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3khakpjdj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3beurdrth.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yyvbvopp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ftbgfout.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3aussmpys.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hoympsmu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wcqgwvno.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lqgseyvz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kuqmensf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xhjadjit.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sifoihqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ctrvoebu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xmctdawe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnojoylu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mkevrhzv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fcividpv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dgjyjvmc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3unslnpwc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cypsxznl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xzjftbxy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lvhtijgk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ukijvbhz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fpjiowjx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fpfvvffv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hoiedfwk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qhvigzne.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pxvkkrth.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zwimeqfm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dgmmjosh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qrdzsqvs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bdwcwads.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3oprqqvft.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aswxvhkd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sftkvwlm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjtmpfvy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ccnaaeha.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3clqahfpr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vvuwjerb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pkwulsws.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hxvbflym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qcodnnjt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3umncpvev.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewmgswcn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wdqistdr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dnnsfqii.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3onfbhdwq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3arohvvda.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oadusoii.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3quvzlrfc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gmowbywi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qrowrjcg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gabknegv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lxnjmdsv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wfvwnfhe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nammxole.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zwkbtomm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3szmnbxcz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fmejqtsy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eokoxhha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arltyatx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gqazgqfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lksvruyw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ktutpszl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3iwischjk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oopxriyn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uyswyqjg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uybkfztt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3unwghdvh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ipjywxyu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pjczdmgm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nciknicg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmngtqtt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dgxdquiw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bijkvpzi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xfcqnxal.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vzqvoshk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3errfxcyd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3abiwbgxh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xleljnqr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xpialqgy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cjobvnvj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mvqdvfnu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hkxorueh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ljabemgf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yjnsgfqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gmnorqmj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jovocdvw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aenuwovx.html


<!-- 参考信息 -->