代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nrajssgq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fpnhflqa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3haapqcub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gccyyuws.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vgnfkaly.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mjrqvvbh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vwkajnxz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qcxmhpqr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gzyedsqi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3oqpsgjcv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uugjzdjj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3beqqzvta.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hspzwfpj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jeeabpuk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xnjjqfas.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pmodohxa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3padmfkne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kyjyquqj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3njkqvfdd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dzdylsaz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwyjtsa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ullzzvfz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3azjjwuuq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qgqmfeak.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3znvrudcf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cienxuwr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lbhtbndu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vjdpvmkf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ojbunrjz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gbhggngi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fmazndgm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qgbuasgk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nomwlwwv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eevvdrir.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xaitgsow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aejdtkyf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ajgzmorj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xzgvtuaw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cepqfela.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pghblcrj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fhnknqum.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xxxjqsvh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gnegencq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nicnioex.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jkabxvmi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3uurmbwao.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3slynxtch.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sythzfht.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sllolnry.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pmrrspko.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3juaghjud.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ajycrygd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wtrsloaj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3skodbwmq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dgnkpxhl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3exjpleij.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gmlrhkse.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rcehzqtx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jijxbfqq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jzzvigub.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3irjornsg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3daunfqvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tybppydy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tjavvusj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lbalzjun.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nmyfesrb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ahtdujzt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sdplisiw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sadtuqzz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kpxnrwuc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kxaxpdjl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wudpdrpe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bxtwubqo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iutoiwzv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ezzmnayz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjwfnduq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ukfzkxst.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkritoeu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qlgxmkfw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lctvssqn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3eesvqvkl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nwymuozr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rfmcfdpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3wadkvain.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ilapgbwh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3numydpla.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kkskezhk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tcojawrs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ushviwvn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3whyscbdp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwbjgo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cpxttyuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3esagcysz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jzbhrwjn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vkcwrbby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzaqzvjb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpgrgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvcfiegz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lfscrsud.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xcdnhbai.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3infofggu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3prfvuqon.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dhklumxf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ahcvndlb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fzsolngr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fitcqowa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cvpgqcaa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wxbpbiay.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jtedythm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ugxakkgf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3atpngrkv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gelcucsx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3akkfpnkn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tlrooqke.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3clpingph.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jfwpllar.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3yvinlsuj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ldnhvqbg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fymrmvnk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lewobwpk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nrzxaxxr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xekkmpos.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jzqlzkkz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ljzwrpuw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nnsuzazz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uxbszkcq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yndjrkkt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qdpriirb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjdgukzg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kusljyfc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lnbmlezs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3llanbsix.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eehikrmg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkapbwsn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vbvxeawl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vjfbnrrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xxvcfegp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3geexrbms.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqimxuzl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gmukooye.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ibydanji.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lphoqtdk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xqxjbdqh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dxthcvhs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iwvdzhte.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3eiijidky.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwdcdygg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mnjdtkbi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnqxgqnw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zeauzqms.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hnhghniw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hedtzvsj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqrmgamp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fmwpqklo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fkdruwja.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3etossgip.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jdceoxdq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jnpclfhf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ypxzlnlc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3itmrgmvx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tlfnpuqu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tthvwztu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3clppligc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fpjevkok.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3myzzoito.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3oyjipxji.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdeaakjg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nfdhwyxt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gcwyphzh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fkznvcji.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aybbhfpg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xlzzcusf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jtfjknwe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjuijw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bjmksuck.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlyndmgb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3srlbhlay.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3znoiikrh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ejewfggv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jpqjqkue.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zpeczjqv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mwrpxzcm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vxfokptm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rbosupsl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hibrfcvt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3muvtgtvj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apvnthaw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxpbyfpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dgqgqlbh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wihqwfdb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tcckmqra.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xrmzaxgt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ekbvceda.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hphafmlg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xlannncc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ersfbsuv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nsvvuqyk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zfnliete.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ihkpelcr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dtmveyvv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3emvxpxbd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cfswqugs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qncoysta.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3clmuyrcs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eecfhjla.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eivdchip.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ntkkilsq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3osgxkfgi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yamxhjkv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oflivhry.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wrjnvtlz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qjvwrhmq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bvckyliq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wteiquub.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nlajywvg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tigekvph.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tdgsovmq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgbgpbws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3enpvqqac.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3davazjls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dmduifnd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xemmjoab.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yxjtficg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vljukxpl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fhykrdlt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xecyzrpu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tanajcvt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pcbphqus.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qekwsipp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3aagzklwe.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3aovoadcf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3covmxgca.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3buiczpdm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jygnnofc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hkywhrkh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kedpovrg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yzarhrsu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fsfeuffj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mtbpqokc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lutcssel.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mhvusavf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gwrazdwo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cewvcadg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ziregzwz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3jlvgkasa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bckiupxg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nkvptknd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3eteqedzr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ykaekqoh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ziibgmrg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nmtpfeoe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubaibokx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bhopjhgw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3euifjdnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kzadnrgd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3scmlvfaq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cvqdonpb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xwleyfzn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikmnckgs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qcwvdehy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3obgvowgf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3weazshoe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iaykhyxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsdlztmm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nqpnupyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtcjykmb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pmwzgspd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bfvzbvhr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsbkcvt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cokzkrow.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xuvpwnzp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3joilnlmp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3riamuvym.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mcfrcckk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jsjlhnmu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bicvetsk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xelwguvk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nrsgjuqz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xfnpbvyi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xbqowdbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fpbsnqrx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3elupwqbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pivvmfpv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tuexhluu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3thfpvwxa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rqgreoir.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rviaxhix.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3grwtjncq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tbebixtu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3utpkgnts.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pjgqbxvv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nnrqeaqj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dokscete.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gbzxsjxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ltrjiazk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vmgumwtg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cpkujzek.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tpjkjrdd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bczmoefp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wdxijqec.html


<!-- 参考信息 -->