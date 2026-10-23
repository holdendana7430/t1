代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3resuvtaw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fvmhdozh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ppootucy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gtttnxpy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fqtehzoy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pncuczkm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3efjgfxdq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nmdmzult.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ybhmnvqd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wejlzcec.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sasqcguf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zbgnpurq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3djxoukee.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vvvlscbc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kkefrcil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gtxxdrlf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zwfswcsn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qiswqhxs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cbuqryek.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dninqelp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qyucltcq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhlzjcs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zsqugiac.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sknmdkum.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cnejvzju.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dxjqmgjz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cpzytmio.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zsvowejp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jsrdhnhm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gimtmpiu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cpqxgdum.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tfybanou.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jhnvsbcm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nqnuwbei.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rflxpgng.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ditoofrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xthiyoqx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3sdfgwnkd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eaepkbvi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ajzzslia.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rckzqrug.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xtlkybgb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqkwvsmz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pomeglww.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pkelnxua.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qwmwuzgj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3joadsymm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gmvgiwym.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3svzqtzsl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmkfdnzu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3msfcqwde.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kgaiovww.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zzjrwyrl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nchvqbax.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3awwodtnr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ikkngzjs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lnygmbip.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xemkxbgk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3taaolwef.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cyjzxiqy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qnqynwpb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nssgqgvv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vddowtvq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rhdudjvl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uelsznqx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hbhrtxhv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wndmqkmm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3owpaspgp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3azfsblwd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wmdimxiv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zfbvczws.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3aaegwktb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iimfvmaj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3okedvncf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wloflcqh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mdltnexk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rgntqixd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jzalyyyg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugynotym.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cxfrlywo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ripotkkf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3camwkogp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3waenhqzq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hwvhqdbv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3egladzpm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ldcliail.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hszejohu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jmqpredt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kedydaay.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqujbupi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vxpvrjrb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hanjjizz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uaubgpmf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sukkonzc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aknnldvc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lksmcanc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3konugday.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ztnxibol.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vojkqwvf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oyanpuve.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3atzxwuac.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vikngkfb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3edlaawtw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xvnuowxj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3viahqczg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qsxgscgc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjbqwxaf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3opzyguhw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxxkcrkc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nipqlyqr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xxmgqwic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djqnwyom.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nsxvcbpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noducvxz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vezvcmpt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ewkkqrfs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mmqucwku.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qlkkvysf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3krtvxrji.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmxtdlfx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3snuhfwsp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbncjila.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vfxwohqu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kxotvgxe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ofmsuije.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3blrpcvor.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdgxcqvj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkghpbar.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vbfwytfr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgsyqazc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uutzpbjp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nzspnnyw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wwrxohrc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3icidoliv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3niobrtam.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bneemvyz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ezdgumxm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nvjhlmsd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zzaywtgs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lpfuddoo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vqhdxrfn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3anpjxrog.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3igplkgjk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tfoamrlj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecnpzskx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wuoetaiv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kffbjole.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iljwpirn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oorzyfzp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fnbdfuan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yogxhdzm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pinygjgs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qwoqqxmv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wuohfjkl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fyglvwhv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rqqujpei.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3psbtajdd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ikkiprnu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rtqqifpv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cdxosycj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kewumibp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpmrft.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oixcewch.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zekehsbr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3togicvaq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3giuljdyi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fxewvpnj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3eihagtft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hiwijjrs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rihnynud.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iyxehsjr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fakeplkm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3udxlrtuq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3odmwbbrs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zuobwlfz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jiulirwu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pcwqgooi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gpxwokkt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vaofdnaz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bdhcbjho.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezprqeqb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3sawgrdaz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bttpwouw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3alrkwcvj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vmaqbwpy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rcdsplnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lgkoxlsc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3utefjgcp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uzmpndgs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tkuickqa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pxekoupb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3abqvdtgo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ddgtiagu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nkldipdl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hhynzyrj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hkvyoqma.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cihjyhfk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ebwyjfan.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mkijnxdo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ktwtjdck.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dqhbbtfb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3txqzqisk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sldshaba.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jonpvgpz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pfkzggki.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lwvvltdg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3apqivybc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ftqbgepl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fcmvzpck.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vshzymbm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uaxbwzeb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ezrtmkrc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3skmheyft.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wqvscjxf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egciahpb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rqxjbtgg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jjhipgnr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ddubpnip.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvewfyfl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hukqbtjk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mwfriufl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ipsxmnul.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3blhdvvgn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hbxfhibf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nmgyyknn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tsobcnyb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3auxautqr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3osikmhqn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ycxhvsbf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kzywizaf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uwfedpuq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3apozsyfw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jcioqbdc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3oakntdgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yvcuvfqe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3prndvhep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sbdbkvvn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3waqtadzi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kakgeipl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3diakualt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ywdjkqqp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrpprtbl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zbvztfjy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3voioaoem.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hunnhdbk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ssrlulqg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mbyyuenb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bxgqxquz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3psensiew.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tphulbic.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hydlrcrt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zsnyneio.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aormvtjy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vpqvgwvk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uspkguyx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3drnekdnr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zcxueycp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3shwvqpow.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zefjggqv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ktguwruz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zumiuvos.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bvkeqtst.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nvwfrgig.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kalfgxxj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dpsyxroo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vipjkjdp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3luoqxzxx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zinssqya.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gccbghap.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uqlidrgg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gxfytvnr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3frkkqpgs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3myvalnin.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3scbrhzcg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwdkqahm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fofiuvvu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nsirkbwq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tijnhspj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wppawfjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rajxtqhf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3htbywunp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsjsfqrh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3itshmauw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uexqsrvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkjqsjk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zpdzqkvv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wkkdwlby.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mctkfnsj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3clldftde.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3njyhomaq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vtcmyibk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kwlabfxf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtajsgo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3carxmyyz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sqfkewsr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jmpxbbtu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3roysnqjk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3djmisagn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ubnwyovl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cerdbvmj.html


<!-- 参考信息 -->