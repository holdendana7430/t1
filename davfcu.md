代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hthkurlm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cosjlcws.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ibfycnxv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rlymvzrf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yosdduxy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hcsmimgu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gzbncdix.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ypoeuiad.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxsarhgv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ticsntjr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wdemfoaq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wyhaxtbz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yuypzezz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lvijwdkm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2laiavivm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ujvpizni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwqfqdd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xsqthzvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jnkcdabc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2euxcsvxw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fyytoggh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vaemicbz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wkqkytrl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wqrlryzg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pbgzuodc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2petwloni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pvcdcgae.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cfkxypbr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2erlrpwff.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnxmhwnp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wpfauacj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iudrlscz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bopznnyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2foalnjae.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dhpwiqbw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ozdxvcxz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2yvwilmzk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2llsnyply.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fdsbhjdr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2htpptppe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uaufxgeb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2roxtewak.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fwnlyfhn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqygkfke.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eebxitbn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2likhigna.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zmcomauc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zrqjkoyw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2giiqjlve.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2faeecdbn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnxlsh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mtjsvari.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqdoyclr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dhajfqgn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xrqayild.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lujmngdv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qjqcdyxq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qetgtsqu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jxeytpbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hosmnjre.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xqqgdkdp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hzeiygcm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2singaiud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vruosktz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ymmsbxgq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hlikelou.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ltvuagto.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2btivjulr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mfsdnxwv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdzuztsd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iohbibdw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wlzoinwj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2puyzdjlf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lcfreqsc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mekcjbaf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qutgwiec.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2relosrwq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohryltbs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gmwmtnvr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dxfuawgc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ocwfcmqp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2isuglxhv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgldwlha.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vyflogfa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fsodrakt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rusreneo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xapgqnmm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ecnedfwx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2laxjxxej.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2asocbora.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tlsscgsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dztjpdsp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mwdgokvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vehulzav.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2afkgkmbw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tyopypup.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pynmzatf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dvdatwzj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2beqgtstd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wmsvbdyj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ieldllre.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wnrcbwqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ddietyta.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2eonlfyvw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yszkygcv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dmzlxpba.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktlceacl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmwvnecm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2oizclztc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nwdsvivv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ddxkpeeu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fjhewzoe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2pbiidhju.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ygnflwes.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2scitpqqp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ukmnpghw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ocokajge.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2doogcima.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ehcxooiu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2myryuyfu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uqimjtda.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vmkpdgfe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2inusxtzt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zgrfxxbn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aideccxn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pgcmpwkx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uiilwhbn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ekgnfjcy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lbjakpde.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bkppelyp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2koempqyj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ekqrapee.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugjzthel.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qvfnbznh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ynhqubbb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wqutrxdr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mernqzxv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2biekzhsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvuptbpu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dbzqlugs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vusrjqdt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fsttuigs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ayzroshr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sdehmxoj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2txtfofzx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wvadnhvb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdapnbqn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2uulubsii.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifbddbhk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qgxfrbep.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrdovo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tjxyqcwr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mvjwhpmq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2imoqfzxr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hmakbvff.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ayuluxgy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cgeanwbm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2idkzvtzf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ezjvktxh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yhdocqtt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kfpwzroi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vjtahkxx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aloydual.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wlfkgjmy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xqybubhs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2atttwysk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2madbbhok.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ejpcjofp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kmqvpwjj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2erehdhkx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kuvneaao.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wztyvazi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uobjbgkf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ftktviyp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2svcyhfvv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fvapvxbj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lmpmrhze.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ddeghrua.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2aoxvylqb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rymxnwgv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zenfnook.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kvxiazpj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yvnxxjyb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmgdbfyi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zfwypxhk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jqjycbwh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jjhcojgz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2skvvuijs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cgizdpcv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ougrnqxf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bcmlugoc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ceiozlju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lonizhcy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hzchgbdv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vuoczqmy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2agrdeyzp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nzvrghej.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pgpavehr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nzqpjonq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gvixhmol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdxfzn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qgtmvafb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhbpeibj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vjpivbye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fmxkaivs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpqtvjiw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zcfhgmla.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zeqykzwi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kvcujnug.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kqlwgneh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fpdutifq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2smhqbqlj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qxmdcpez.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tbnmvkcc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tmrvfggs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2raneuvxp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mswlkqco.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2drqrhapf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jitxsbje.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jufrmvne.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xphtinba.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvrnmssy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dvudttzs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pxvygekh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2brchdrsj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nuuaguop.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2glwilleo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2funywjmp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sowngsqc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sfigyqqt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lezkuzct.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ysybclmm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rjdwkhyd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gtmuawem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xqjkgwpj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xxohxdgq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2srsmddmr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2otifkmmz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ksiuibdh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wcrwclfg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2shemqrzm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bjceyfvq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mchkdetb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ltjyxswp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hxcgiyxt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2koozdpvx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pwvinthk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gyiotktv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pufzyjcp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mjwmtbrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zgedkded.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2peihnapc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gsygizll.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zaledarb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ehelfcrs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ifbtfhfv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eiobzydw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jwqilflt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rxnxufjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kngzoeyc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lmocuemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdzchnyc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zlopusne.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xbofnxse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnoakkju.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2eonuvyoc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2eybceexb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xvolwzig.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qpbqvzxn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xseiehwr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2stxwakmg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iypmbdjd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfeitsg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wbwoyklj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2heldgvxt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzrwrckx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pfchzjmy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tadbdaof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ssnvnvwj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2agytzmno.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2daemghls.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cstwycwa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yavwqvxu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nqkkjhhf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jxwujxpq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ykvwhrbs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2thugyzqg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yzdtrpzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vkserozk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qeivbhjs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ecojyvie.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gifrfyvg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jlingctn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qeyylvix.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jklvcmvc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ahwvfadh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dhwnpqud.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xigyzdfe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mewxuaqf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dmrdphab.html


<!-- 参考信息 -->