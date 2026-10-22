代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2morpcgza.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2litmpkvu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jjphoivl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eoclskvl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zxatumic.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vbuuarce.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2phxigsrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2udlanvag.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gtoxulzm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hsviiszg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ugoovttj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nbbnknsr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xthsiruy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vgmeaptx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xgfsmeam.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cvurbrjo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2mqubbobv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2uahsnoto.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wuhyyobn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jijyuisv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gvwuelgh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wlydqpbj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xaytxrid.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vdnvjowq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2azzklzka.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ohxebjvo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wcqkwuny.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2idhvyngt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjqvtlrq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rapwblbc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2queyvyhb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ghzmgigj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lderhrnp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ccieoeft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hkzfrvou.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vaqcpeob.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yobzxval.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fefwvife.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pxuajvbe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tseyaldh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jslfmpei.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2veipnnry.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kxhlmuxz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2uholpfmo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xwkdebxm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2euxhypuy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cpkjzrve.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2votnmxzw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yjsjtngc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aiahhmxt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2usvrswxs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rvnbqpwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ghucyxzs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pkbgtcam.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fwnkmbxt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zpydzgbx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wtbujcpv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uvvaiqdk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lzarxwos.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xbydevqa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgkrwrsk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qvejrmdd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fnukzpbk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hsdnqjpy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2siegxobx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iwficpzo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lftsufwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kirbiiye.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rzblzdow.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mbpwsuhc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2gacmrgbh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jtyqnjzj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bsgvjfff.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wkzzthfc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hyhxznrs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eeshqegg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zmykxdsz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chfdwhze.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2huiugwil.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2muogdcuy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcjqkwbo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hteiyucu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwozahgr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cngsznmn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iagwzbtc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2poxzvpxu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wpfoghgo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lwzjezpz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tgpdrwtf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cyaudcnr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hnntxxbn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2whzkjfzw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tctfcvqe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2asahqxwz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pzlvdzde.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2coczjqwo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hdoqtjqd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rmsoivpx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ekknaktj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rswqvpta.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ndxqfzvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aetvqwve.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jlkrramu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ooxlmoox.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tvjwnzow.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2erzbrrqa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oehltawo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ycnsmebu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ciwvxjhu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rvpecogg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dnojqeqg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xmrtmcsq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hwotqwib.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zioekxcs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hgmngqmh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sakpgazl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fhrblobe.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2unokwxlo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wotbiwbr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wnlhzkbv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tyblpfby.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbbosfot.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zwsebjxf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgmkiwtf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mjnkmytc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hdesktku.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2okwhyaju.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cabcalrn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tkidvwtd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwcwuiyf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cwgtkxan.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tueedjzg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwlnifvy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hvkrzjog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ikxbcsli.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2abyptdju.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2stlmwcio.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2icviojxo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xhcgqupe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nhjijaxx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2izamyses.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dchleewv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xoupvsxb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cgmdchfg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iquwqktn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ujsisxco.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdzrczwp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ufezjprj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2upjpthys.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2phjaacek.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2otcwbbfb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2njryouvr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vycrehlw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yndtunzg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kugxipch.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ewaikrxo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2itzxphuf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpgnjv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2faofuvmj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2thbaoacq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ikdxmzco.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sxwbaiqo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pipxbjwq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pubqqose.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vnfzbogx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tknkxviz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2spzuacmk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xgkkgqdk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ebqyzini.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kuxvmokr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oqqojjeu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zlcjswsu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjhdhk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ogxdxblo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2prlywfsy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ryptqvwb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xtpvitke.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2voxvznuw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2uiictgba.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qpthmhww.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pogqidjr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hhcegrof.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qsoeenrs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lkecrdwz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qogftxya.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ylmxixho.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nphongai.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mjifbgzc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hujnjzop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qibdtkgx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gptwdbbi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lhkholkh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gezdwgqo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ebgwbcda.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cdckgnpt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zjncvnem.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gptewlwk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mhpgwmph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gaukwgwd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxmqbvpu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2whoirvbc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qmsjgofd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kocquvjh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2sbjeumsy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kznlfzpx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ldgudlxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ofagscdt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nqjlhcru.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fbcpvpbk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kjdtrzzf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dzcukuup.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ondazmeb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hhcjhjqx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iusqzzgb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wzeujrbo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qtdstsrw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2atohyohx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vdzcxfcm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2grkpmbif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nsmbrzgk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mvnltnaz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhioqgkc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bwegpvip.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cfipslif.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iuebqqmh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ybztribv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2olkwrihv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xrzesgyg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2spikjjec.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dcvabrfk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xaxjfwrz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2knmdppbn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uzozppot.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zdppvcsk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bfqegcjh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fveubmeg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2njcvvtjg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2djjonbcc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kiwjtvgb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rcjrsbzb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fhkbucyr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dwpygfqw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxfrarxl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2twwbpyft.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2razlcito.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2axolcqhs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rxcuqzru.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lyhlgpka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vwkigrnc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qyfigcrr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzeupgth.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2entnbkbb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rfgcixhx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mrasimrr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pcvcquyo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vzfezwsl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lxfsskex.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ryhtsrbk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ouevsdot.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nkrrsrsg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nqmluizl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2snurglxc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rxmpgozv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2viudxytw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mbvgjcye.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2raoavcen.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jsoumrjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fudxgeqa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mtehqzos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxzawpkr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvmjdviw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vnhjmtam.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uxpyccrc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kwjdugjz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qccmvjhi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zwjrdjjz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ljoazamx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2usmlympm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xwnimvoi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhpgwhqd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oedaqzwk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfckhdtm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yfywlayu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ustwgfkz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xyedcsis.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hsawzbbn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2skdpnxsf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qaununcj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mitjjjga.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gevdddrf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jajeldfq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqviyjjm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2atszpgdb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2airbxymk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yahpsvet.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2epriufgt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ggiwpifa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mfirhhzf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ogyyqdbo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2prwrblew.html


<!-- 参考信息 -->