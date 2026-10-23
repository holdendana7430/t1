代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lllszueg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mrpvgzsx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3yggmkejn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ntlwjzhf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ghzefjnf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hyicwewj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jddjhjmc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3spaxwdow.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3apvdadyr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3phwsjlbj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lboatrkt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3sdccvbme.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nbvezcvh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mtdorqzs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3krhlorvb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yaklagks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ivzmqrtw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3phqrpnog.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zbjxdcbx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nefuynmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xkerxhgg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jkastugb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhtauth.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3acjijeek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qzatbucw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ukrcmjya.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xjetrqjs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3htzctkti.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3upirrnen.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3plniheqt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wzkxejtl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3grcbexgr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3stomdznu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmurpz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kvjrcnvm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3iigcoxob.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3utpjvutk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nhtnuudx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fcxfqhxg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tlloztjt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jjdqwtpw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzxerja.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ohlkjufk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hufschcp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fezqaywt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nogsblaa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fgrjzkqs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3htcoucpd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uulzgkcy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3puxeqbwl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bixhimen.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sqchtrek.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpbrwwnp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gnraieor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jaeafowh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3izqjiwil.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vzdllqcw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sfssedrf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bbgvtngp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cryhytjb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nxlnagtm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mxwmjdjo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rlrlhenc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gigozeep.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pleqxivq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vzamnzxx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cpdeqkeo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jhtvlxag.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ajvbftza.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ormowvrp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kuogjunt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfbtpfvx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdozgbom.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxtgkovy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yciysfef.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ssakgtwu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yldvsegf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgerdcvo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rulivzhg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ffkdsdkq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xshgsmdn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wrrdccep.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3szdlcldi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rkursnyd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jfpcaxvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3quqggbay.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3saosbjgd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycgqlwlf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oaewqfjs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wkmdeoqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gtxkamuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qboqnsvg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ckezgyjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeubuclq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fywmeudg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rrqyljfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rslbaicp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pngvroau.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3visqgaaq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nacqdcim.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ffjbgoes.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xvertawl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yhpylypu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zfuvttvb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ibbbnlhl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uxxxvcxn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkuihfd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xomhowls.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xomdifkw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzctmiyq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nvpjlzia.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdaaunmg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tkcvveec.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hgcquagn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wavcheen.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kxvqrmto.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xgjyjimb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3giwamnxl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tpiqlxha.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ukqysuyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qpnstmfp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxayttrg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqqoxoqf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3avmvlagz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eqmeebnc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jelyageg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nkhwmokr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlpyrqta.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oasiirwr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kfzrrikh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ojdrieki.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cydzcokg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3majqmcwh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uqxpataw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nhzzhlpe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rmmyjdyx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wwkcmqsl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qwdftdln.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gtttxpob.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ykheohqg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oufkhoua.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yyqvzeyl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ecqdaxdz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bzivljhm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zmopufjj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kfjunpmi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3chweaucv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vncbzfur.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hvtludcq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfxigt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ocbaeiyl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3sgalhksz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nwkybgga.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3hdlqizjl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wbmkdlit.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlwqgyhp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jjudtmac.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rgjfxmbq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3baumques.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ymbphhjr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhjreqa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3oqwjcsso.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnulmyov.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kuadhqjb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dbwqhawk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xiinveov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwtzemup.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fvyghjpy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3usacnune.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3trtzgizj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vpjojxqf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gheutkbd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jicwzkor.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kbfxjkqe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nafntdev.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rsfqoitb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3srxnoksb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3prbmtjhr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lcgtvlhh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bihubqyr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pgmjrhwa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3osvomnio.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fyvfeyes.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xghwnkhv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3csedprad.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3guvfwgjb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xrcdjwwt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aifvjuhk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3slydnroz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lnxlguxc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3exmnibnr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lweobdfp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vsebjhul.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yzeejzav.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjbhxesv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nvygukbn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xdixcivk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ttnexebm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pqnamleu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3njlaeefb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fseblvtx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lhhspfii.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztmusxvt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bqfqrzzc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ohzcrizi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xtnhbgla.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ouhntjyq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3enbqjpqa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xbdnlzjp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nlopbtts.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xqcqcful.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nphjjpdm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mouisfmm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gcwvmrnu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3twvadjph.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wcksppsi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqowsd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wpuqdnpc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3usbyenie.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3aqjzhelj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zwtvzahr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gdghpvly.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3sgdgyhod.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ovfbrdur.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hqmjbovh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mweijbbp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3usnttqdv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nwcsjomk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mqpfawpv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rsulcfyo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vrxbcvwq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iqaiqfuw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gsqevdnr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qozxhddw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zsymrgcf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ofsbjaif.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gohvcjpy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vcmphlvj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cglswkko.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xujtfmof.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kdippxmj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jdlwazzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yermbsxn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrfwkfej.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vtqwpcne.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xtydvgxa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbfkmxmc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kfpdluut.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wretmdyd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqoigzss.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3srgacggo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3yupuydlx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ujhmhywi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3imrxfunc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3oxhszlkn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iadfzbes.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cqeizigt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3chfzmxbw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kxyesjjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhnsykua.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aqaiykxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmpkfpne.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjsxfqtd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hwgyjbiu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3krtrozgi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ufeginrq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rnbjdlps.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gwnqqbni.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bzppoziu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3signcxvz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wmaenpwi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gumpndcl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvrfenl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lapodjqy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bgkbedme.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kflepuzi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ceawkqdz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3sxbhrbvs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tyhqmbyh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zmbeaihk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3oexalubt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bakkctjg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lflefcfc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gchduiig.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rvhjcubz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oijauzmu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ivumeqnd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjhygswq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gjsvvnjd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wmukrkjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tdqhrssq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lqtqyoem.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3blpvsjuz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvzptqch.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hkqrxrmi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xrwjndvl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bzkbefch.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbjempdw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vbbwyyjg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xsdqneuq.html


<!-- 参考信息 -->