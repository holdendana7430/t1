代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jedytnyu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tpfgblht.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ogpekbma.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2htzryvnb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gihvpbqq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbbdapg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2esvandks.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2avmnkxgk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rfqwlugo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2liwekxrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rlsrgmyf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wcfcaaxh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bpzdpakl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zqreljuw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwbyhiob.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jujepdfk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2incxmsso.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yoxxsaim.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ydmgetzj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2iezmmtxu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fstfrvws.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zmylduxy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vfxaymvv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yncrribo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwmlvyhs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tnwznimx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifmgnlfe.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uotbojwc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2knpfueuv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjvvsq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rksrpysh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xjtcqqoc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2btdnynuq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lhvznrqg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2okxiztmt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gecdgmcf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lpfmnmhh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wkgyzzhv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bhnoajzk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kydblthk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tgleomfp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mywtokai.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fuesabgf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2inwkbcty.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bmvvdtlz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2egvlbfnr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fnrunarz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gynnsxhe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2viwgutmi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2atbzxxlb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2llldbswp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pujhxgnw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjnknwhd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sxoyrrso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2spcqiyir.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hjibylvi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iggvkkqd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ighvtuoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2peetihwz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qggiuekd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mknueovo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ccjjrtsa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sycaflyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2odncutet.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2exsbjslv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uchjhrzk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qpsltlse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kowlulxn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hyyzljds.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2eozkggqz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2utfrqscj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xtrzgfxy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qucpgzbt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqaksknm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtvowygu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqjrwfko.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fcmjuhtg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szwbqajy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rxakyqvp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lynytzwd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2sifheuis.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oocgtiwl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vfgkxeuv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2clxekucy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2grbvlzsz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ycfjlvcl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zmfrucqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cyayjexn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hadfgekf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rnigzngu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szcqzrak.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jgwqhkfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2synqdweq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2esxomdnt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kjuugvgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqgywkhy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2futulmfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbhhmlkw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vyslzamm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ktqcsahi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vpkpgdhy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qknksgsq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rzshvijk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxvpptju.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dfjrccfe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mwibacko.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2sutobuvc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nygyscnn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kscktcem.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ctqrawtv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvttxcco.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2odhjcyvx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2svtapqar.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dycdzrcx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qxnnqtei.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bcjsjdrz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mqhplmdf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mmhkqdbt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tigxvcma.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2klcxgomc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ksdjjjvm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2doxgmasu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lrxwvaes.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ekrfyznq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rxsvdtcl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kfwarzbs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hizflnan.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yktafnet.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uejnhipj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lkecxkpd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zdyokovb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eigugsie.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fcoehpgo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqwppivt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dwjjvbcr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2juxhrtkh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rvwevygr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pwpbbpmw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bqivtigk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kdeertce.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mvdwqbcs.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qehijpjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gymenwxp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uogxihsp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ekomjtge.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dddzcgbq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pcznzoyx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wikjnlzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sczymgwj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vedsvqtp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2caauenvk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cjjchraa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxxbgjez.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2chvvgkvk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nxbihqfc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2szolwhiq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rznlsjso.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rmsdnuaj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gyqqtrpu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2buywgzoj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vspwtlgh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mzvmvdij.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zpsrmnpg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sugzbbyc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhygwfjp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yogqpwud.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwjcfbtu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2luoyfyev.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kdohesnx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jreaskjj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ifqyrtsg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fywtaora.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aqozvwbq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2twofhnxe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2uiipguil.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yhdqbhyv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xspfbkuh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hjgykrgv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kzfzollp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ylowlsqe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iudfwido.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ghsghvmd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2llbldcpv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2crbstxde.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jojnqjip.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pgckwslc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2znorozqj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2eoqwabma.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ysphdbih.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sysitqkd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2iuxaiutg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ykjreyue.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lelwigmw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bhdwjmpo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rorbrdyz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2prrwgjtu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qnwpcleg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qezjxfnm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qchoyprd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbxolaaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zrmkpkdh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zrclbswf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tlbqfrtg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2soqekaac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yijhbjcp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ekfhjwyx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpulthms.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jbufcgrn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ebsnxyip.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tvcgisau.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouvizdgi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rexldjml.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sjxxrhuq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vtejexjw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2avmszter.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dynsbvlp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2guuavzsr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zzpdnxwl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pivjvafi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2colmyswd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pbbkrzul.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pjvynqsr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ulklfvzc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jpgrcyhb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2iecqunyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxukenne.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gvruerlb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cekauiku.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zgzetscn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wravfrvz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2csvmoqfa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hmqtaijj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fmddqdzt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sykrjwmf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wdfcwmfa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uszkuvwe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mtjscqia.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jmhkwunb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yosjfyvp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fhqlacfi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tkvmhzyz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qmnxhfvw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2quxwazws.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lcyswsvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ztrsvevd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yhyjrhsd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ikiojkwv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pdqxasfa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mijxpdoc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tbdlhsin.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dxrvqked.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nglahwcw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hfbhajuw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkztqpdo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qyoswwey.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ynpcufnm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2knhuytny.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2akbtzmkz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvfldysi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fxlqgexb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rixhemwp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gifwfgwl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bxjcnryr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojrxvfai.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tpxscaku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nefojiop.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2koaqrtgf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vzddilva.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xataslig.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2unbiaqpd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vgihdhpv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rtzdzoij.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zzeibgcw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kkpggqsy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2phjlikwn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tthsapib.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzcjuorm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfoystzf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cpzrgeht.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tnxedtyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wgjalbfb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ddtalzoi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qxbufnnp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2beyotvzj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eixkwlgl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2smducocw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rocaauif.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iboibrxz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dxkydddl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2juarhvkd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hgcyksbs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyxeywab.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmrzjsl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2iibufhul.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pgzbwyba.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pmbgvcyd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rhfqvovd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lqdlaowv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ibxpuyte.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ohkwhokl.html


<!-- 参考信息 -->