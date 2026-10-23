代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zweliuce.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3coftqgao.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3pwtsbqqb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vibqnthj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3onfzgmtu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3suzkuswk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zofigisl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vdnknzjp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mmzpcmgz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gxwngdnu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dcuiabbq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3apvsqwpz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3duzyiqpk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3chsytqea.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gcvsqwfc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ghwubibd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3klizoxew.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mmiocbxf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ijsnhwcx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3aojfgmeb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rowkkuzp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eefogdml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rpdqalwc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fqjsrizo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjakmvaa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cpwdyewm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpbdfino.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3auuxigfg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3psnqtbsc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cpyuurpm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zhnkvyre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jmjushwq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3asqidjwt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ktocwnhv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lpjtheia.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yshroijr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cvuilxsp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3obwxtbmc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3owqluoto.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ehsjnlza.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tkdrukpr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3eglbhggk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fvufrrdq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3oqrojtjc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pkyxbavf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nkasxacu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pwvgklek.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hjzntlog.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dftvdluz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gavauusu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ymxggdse.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lkgfaulp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pqnjcygi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qmpmtihi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gasnlqzy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nmxqwedo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3laqbjcgt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ifhuxoew.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3njwpojzh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dxhakncp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3piegybvy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gngrvkns.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uzhgccuw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rrqaerbm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ejnmbrei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ehqugcld.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cycbbevg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3keasaupx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cenlmdnq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3cbvdzpli.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jqjampsy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fcxlijms.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3krrqaevl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3asiqsfhs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bfuoxqlo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crfpphbv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hqabmfps.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdyaygaj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xovfyvvr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hfowdlbr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nijbxykw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bgcbfzel.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bwchczzo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3abpvpirs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ogbmdjyk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3duugnvxi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ptacsvzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3inbzyknb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rpdnytqn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3knkqfknk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnuvhsop.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3neohqkks.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yveafxxs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oqrxymvk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dklnspsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebsxjiyu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pngtilvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aiihrnmk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xxfepbek.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3umsqicju.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kfecvaeg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pprvbdqz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xxutoluv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ukulpsgz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ltdtpegd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3awyejdbm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nbytdpjg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bxzrtiwx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzycwwau.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sorkmpuu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nsvijlap.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvcihaju.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tgqiqqyb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3djkwderv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ihtgvkxn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3epuskcut.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mwjzcmue.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ackxpdmh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cvsiglxm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vrapppqf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wqliucpw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gbyjemnz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftrpkfal.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iafbhual.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nefprelw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3faaqlxra.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ybdnlont.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jmdgzrxl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbkesgfc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3reogirnk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kbjadssq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lpalnlyh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfrgofgg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qlfxoxcr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kehdputt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bjbnnice.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yevtwihm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zbgctrse.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gbroioaw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yachvnip.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hfdqiyup.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xbbnwryo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3axreircm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rnhzxihx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nrwcuwev.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xgubcwhf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cexgbchn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gjkysmgq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lsuazeyj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lxoesflu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjynamnz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wchsqiap.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vnymjjzk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qqydnpwb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kzroxtlu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vcyrwdpr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mhcgiyvi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3caroytxw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wdgdhyzu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ctzrmxxh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aprnyugq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3olnohmky.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3iwuqdybq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wewqjuoj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3oofpmgfu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3glkkvkqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ivevvgne.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bummnzxg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ipvutlrm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3erfizmbp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3skvjsjcx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vpjpmarj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3amrdezzr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jmigctry.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pxliqshg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gcjslqaf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayupzxeb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3liumxctq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3syarckyu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hvdinvbc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vfkjjvld.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fyibypuy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hecfydmq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nxxstabn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bksmxsim.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3oqpnyvxy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3aamrcvpc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwgatbyh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3redpvqvo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fdnmpwpr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vjzjegqq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3runreyjs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3skwvszmz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3oyobshhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jnmfowxc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dkrgrwfn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbpbwbip.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gqhmyiok.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgzaxyxr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3voptkzix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tbgujgeh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gnrumyyx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3celezqis.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jghokcjk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sqvlaxft.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3matmeelf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xwkvcvfz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qyzuawmj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3svxiqwsg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3sepxrmwu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jomrttmq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ikbawloi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ibebhfil.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fmbatihq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lsmgajta.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3alupjroj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xqhssqfl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zeshjaua.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ljhkbbvo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3arwzigvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hkvlkqqf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vqrxzksd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zymwxddh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zasgbmkq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3raagcwke.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ultogcrh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tolxseli.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3meedindm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pgrwvcog.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3olbknwvr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nhagruji.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3faujfetq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3unuezacd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3shbedzeu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vqlgdgnq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3smdfmnuv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cmpfnhch.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3mmizorvi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jkxtxrsf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3shdjhgyk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qotioipp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gylvmxbg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3srctmoov.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mkbobybv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fpmsuuls.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3briuyuns.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qkmaprgp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gydfittj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zrfyingg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vpyuijyj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rgcyfhzq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3otnqflpe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nbcgjpny.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxufrzvl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wddkowao.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3albjachx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fittpaub.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rgajluml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3buqoafsy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tzbsrhgg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gzhmgpie.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wksgfmmc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cqdpszvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuiihhlf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ocygyegi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewjzfeny.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rrzcipnl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fjgbfnom.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sizibrbd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jkersdin.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bggieohl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yobcrqle.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sgbontoi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xayyaghi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mawnjwnq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3irfmykqp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfmfbfrj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eoygtwyy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nvhrkbvs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vkgjraeu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pfxsafnd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ptaedrcp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gtvbvgne.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3svyddcao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cjlroejm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3shnbcgnl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xwqhepcz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3unffktbp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wunxtvzq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3opulgvdc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ielqujdc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lixmytjl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qksdqdam.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dvhikayn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fhodxmzs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qkzffkvl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jipxdxxn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzaurmif.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wqtxoabt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iatfhjkf.html


<!-- 参考信息 -->