代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fegyycja.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3swpjpoar.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xpeckoev.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uxyamuag.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vsoqtqvh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wdtyacve.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dxortzwb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3inafnarp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzsnskkl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kpbekgzy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3izpheqqq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kenlgpkg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3trykgjzt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dafplowt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ajfwhevh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3exctbons.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3otadtfex.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qakpgrdz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3totyraay.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fljkdpbg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jbigyoph.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3edttxyuv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wjnfsrgp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3bsnabbro.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3raarxkeo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3niegrdnn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xzcaakcx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dbcnjxns.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ikibtrkg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cmlehphg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gpsddrla.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ldifmowe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xgnwamhe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ryjndhlp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qimttldo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pfmzuiwi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3uevybpji.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yghpbgju.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajuaqfmj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ecvrgvme.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nwjvnczt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fnnusccb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cysmcord.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bvwdhaxz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3umuzyill.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mnnawigj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dxhrheey.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ouicwfyn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3adywqofj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vgjppuat.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3darvggnf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jlfmhndq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eboedpsw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3odowiyor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lwwgxqmf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xlguhkdv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kdpcveck.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wenacckg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cwpykatg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cmrwilqs.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3eamrxchs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xmmwsnwg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jjxnxihk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kjylgnbr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3asekkzos.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3povnlirn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hvymcjhp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ouswfiyz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3arxpacen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3imsijzlq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojsygctc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pkyzvbsb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uviblwwy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eadjjlbj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3keliaoba.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jpfctudz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cwzddrbj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqoqezgg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fwqkfarw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3agfyyeyn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ffhrodur.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbdctr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ngetpvya.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rujkrzxg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dotmjbfn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3glyqqeop.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hifddlmj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3luixgkhg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zixneogo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rrimhyms.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qzumwnbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qudycxmx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3clasxkwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiiihnuy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ecibcnwn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xxgqgbqc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3raegoxno.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3egovzhzv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hptvwxee.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vrjoorcn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qvguhirh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxtdhaar.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ebpdggpt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3blgklvui.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gdvntlul.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ulzajitc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uzpeqbet.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3aogvnsro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fsuhzyxt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tgxdzibx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yqwwnojn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcxyxfnx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3chfyherr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3erehkmay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3egygothp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3klnkkjib.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3txrqhxwz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lhjesnoy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zxdtpzup.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ogkyrxfn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fncxghub.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3chwvdzvr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3snekpsrf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eigtwrmb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hekrdvvu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ahpivwgo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rgqhyqeg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ofmpnbls.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vernwxkd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qzjtebhd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sbechreo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nzhlwtby.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbhjekxl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uyuekrrk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rvqaijbo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zaoerwcp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nmftvnbx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gzhohliu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pkheojxn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vlebdzjq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cndlfivs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xltgeqjz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3loirehbe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gbeaosvb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vyakqqcj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xwlqmeaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tneikuiz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wadarmae.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rptqsfgf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxzxfaoe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xtikdedf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zqjhafpo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aibseckn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wkrujzpw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3uvfgzjef.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kbknpkmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wkustcyi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gmjnlkkf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3epjsrltq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3spvyvvcy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3feyhmgic.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3huccnwcs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpayzuiy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3srokmbyr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jlfkzvzr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bbdgkuzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mkxivsrt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ewcocxvp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wgldvbmg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3eejkjkwd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tdjzihcl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3baawmqft.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mxchazwd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rcrdnhsa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bneetnjw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3heiepbgg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yqespwpc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3acnnwchs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dtblskho.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lslqlwxa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ajyhnuuw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ciakuboh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ywkakfnv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lvkxeyvg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ibdrjnoo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zfjeqgvt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oxooqxcf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ogpqlxny.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3apgvvohu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wwnsepzd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zwrppihb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3thltdrrs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vjeihzyc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3blvlcins.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bykqxuxu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fzourglc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nqjejukr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tktellju.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fvaxsexw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kupnhtqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3acarvtwb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kozxdpjh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbkoicnw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hilfvzff.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sfrpaeqi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pcvjqtkz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pkflkldm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vqqbzmai.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yhnpclcc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uqlqvczv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3omxmpepu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vlpqdprl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dduoghej.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vqswvhmz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eoblgtgl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qwgchlvh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bpjgvemh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kpgddstu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3igemiwfo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xsrfrfop.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iyqmyvgx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zdhfsdbh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vlymtpbm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fmawtpse.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cuwpeukq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ulikanma.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqttncv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zlnrcwfg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cpmyysop.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gekzvdqh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fbjykosr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ktkhllmg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vepctdxw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zmrvkixb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3efjmmftd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zetlhjvi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3slbxsvte.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vductiga.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3dludskrg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yhgxggsr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gonlxryk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yoqnznru.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3envosduh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kqelxqsw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uotvezme.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gnejpzvd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwlamkxf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eeiguoci.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pybkvryh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rfeatzuz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kxgpuioh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3arcdlflz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3otrvircj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dlomwqfp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jgnslobj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hnblpdpe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kvfcxalh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bbdvrvgg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mmrjuwtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvkounof.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zyjnfsxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hljhtprk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbltbygw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xwyhweog.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfrxsjuu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3unssjjwv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fgehevpp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xmepebdj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vdvyrmdz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qrzvrpdx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cygoqomn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3avjnoyqy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3eqfyhkvh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3puriepad.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3iyintqsv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3otppvove.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3izjpkkyb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ymawnkgz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcjbnbb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3felouidy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rghksrgx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tvzykdcb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rkurkqks.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ppbyrknn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xijmjhzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3exagnlwl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ehueyebw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwzfarii.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uykxzpnd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jzwtfzih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tlkeuclg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ohhpffib.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yermygsn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ahsohdqb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uymefpmq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rzclcnzp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwhmjku.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uanoloov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qapveeol.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gtsmuxen.html


<!-- 参考信息 -->