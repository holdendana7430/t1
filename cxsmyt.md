代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mazhaqmh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sagdklol.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3aucejfyw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3drrbkhhu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3keembfzg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gyluiuul.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nagfubyc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nmamosmg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kydnbkwi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hfifievs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgglzesk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hgtrxehc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ebkxehwi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rrycqsex.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qstnlvfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdjyqxib.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3npiwgdqa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cgbedukv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sehsgjzf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3adytfbdl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zlmzgpvg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3emuzroig.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wqtniglt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tuqnwopk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tegpfwbo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sdthromv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nesmdhwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3neqawbgq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pcadpdfi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vsnuthys.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3jkwafwcu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kokvfqwg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cytvpncz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjiwfk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lrvqqdzo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wsjrogha.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bgevtdfj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bfqghpdr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wrxgcgtn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vypqcded.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uyskdixj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fmrfkney.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rbmphkhq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ucwtomfu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jpwlgtqv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yyaqpgbf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aoulazyu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nokiipef.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iiazvlwu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hohwaqfc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nuqpzbgx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tkszqdpn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3byilrjff.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gukojmyl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vvxmdbhb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rroaykam.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rycpabub.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cdmjkfht.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlrzhcaf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3diypcbof.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3awlnvngj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjybmhyy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xbmzfadf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttjkwzbp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qjulzmsi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfnnkeib.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zmqvuxvo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qyedfbwe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3isihgwse.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ucggrrpf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qtcwimoo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3avvlitjw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3czgafibz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tbusumjd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bswhhfxd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jgdkdasx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bcbhcxdy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lronisyc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tqzyjbqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viltkmpe.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3atzbfdut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyzdigpr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jeblbtua.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3drchwowo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xyvjxjmf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ayvufqzd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vedrwoim.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3szikkzdz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kfctrjqr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3itoplgfl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uequgirj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ztgvaebv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kimytrvb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sdqqamhx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vxwqqttl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ebxnmsyw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ljonywtz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pfrrwehu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ndycsrmu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3arojaaqf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3yulonflk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wnrevuby.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jwhnbkcq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cixedjez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xxxwjowz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sesxufcz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nhetmafv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zrquappj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bezrthtl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3chebpxmd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cndskswa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfvqwzbe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zdygvxkt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qqdmnnbb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ryxyjlyl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbwwdpal.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mlaatwuw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qwvesasd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3brlunttu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fwctlvak.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xxxyexco.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ijivsuac.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vqdwblgz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xejzqggm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3naxomquu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ncqjpwrb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kwvyeolz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vfpxueus.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxzofanc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xhyqcbsq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bbtrhkpq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofkwsric.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qpskmoae.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wogropwl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rjcjxqbk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kftluqgo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ysvonmsj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yfjowkrx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lqgpnnuj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3huoyiimj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lunjphfp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sjfashhv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qsddkfuz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nsyafwif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3agxyzmnm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3niudisll.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nixbugas.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nqatbvro.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ncgobvod.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cnpqjjhq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pmswzkxp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ydncntqt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cjxuajdm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kzxfzlhz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qgltzwss.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cggjkmkw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ybnmjbuw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pnofocpn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fwmwpglo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3owyjbhxh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvsoygt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ejgnafga.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vyuovisf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wdbigbna.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kndnwfvy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3amsvrusd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ofwcybvv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hyxabpge.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sbrhklza.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qfjerhvn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vdtwsfer.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eygesosi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bwdbznih.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kwdlnigd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qtjpmdma.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yahexxik.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3futewajh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qxqhrxsz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qvwjfsgw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmuyis.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3szrfvqik.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xisxxjkp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iydoubgt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bgnifpgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pkigynsg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lgbmbzsx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cipkhizd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ybujuxwu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xebtyyve.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hgunmrrc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgwgjmdf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xskvcuif.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bknepmuh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3unpgvolu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qqwljbze.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zgdhmchi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zmcimwug.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rfiiauoz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ifaajrjy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jneymbpm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uynelfrl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xvbmdqfz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3iwumvega.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mjavarcv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mdpxucck.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nmitvwzg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3khgurkkf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3npkditdc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vntewshv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3upeqxrss.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pyjqmnzi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dddqfelu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ggsphfji.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3binmjuox.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uwfwvlcl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iompufva.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kdbnaeiy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mfoemtpr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pkyuutna.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rabuiivy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wsiwustl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3athnbttm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iwrcgwle.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rxocinuv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gaeehqyd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hpwvdeqz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3czrzrzfx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oczrazws.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qpacpame.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wffggeyt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ulgtewxv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ziyimtgw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bwronmnm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gdsuuhea.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3aklvzgjs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zfoxtbxz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vxcvzpyb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uljlfvhr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rollkngv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fxvhtgjl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rrjzuicn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ancjxeyj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cclxkhat.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3iicxyptr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3inndkwrg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ftxpwfqe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fhysvxaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjqtcexs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oibwvpgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mickzire.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hbzegvhi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xltrsdjp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3asoqyhoy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fftlybdg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3axetltpc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hdpursip.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qambptty.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3anepuior.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wswkahna.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzwenkbq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxumege.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ajvhrgww.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3awccdkii.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3iymailfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nyryaowa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3otltvzxm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sophmegb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ggswrnar.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3syasczji.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mfswlxjt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ahpvgoom.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uungnynd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pxnqvceu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ffhyksvl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kwwkejhw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mhpktcds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pcshsrjp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gcxpiczq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wxvwvpce.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gvellnhk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dxmnxpdz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xlmzziwn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fkgmkhnn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfhekx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3idipzzyh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xxbmtvjx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ctaaklof.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmepuqjy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3msdgtwrm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vumplwti.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ihlxxmvh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gbhkjwfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cwaohssc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yfbkewqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tnpeqqzr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bcwbkiyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lzowwtxo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kcrjxkco.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uremxcvl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3oosswyas.html


<!-- 参考信息 -->