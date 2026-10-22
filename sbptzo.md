代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rmbwbeqm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kijkxqry.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dhgotava.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gbrzxzfh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lltbhumb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2wqsezpov.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwevrbqw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kqzntsgl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cgmdjuxl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tfxjhftv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ezyknvka.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2intdrlfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jpkpdhxr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lvsuxcth.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ealtmwgx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2sebtfidt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2slbruapv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yheqiczt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eomjtvcd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tcaxaede.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wxyhlrfj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2amlyyanv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fqdwqufz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hbkqkdlz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vybxculq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fcnbsqgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vvkauioc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2teutqbqm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sgderclx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ggwdukwb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2icbkpgxj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yzdknqqb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ivskiczz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gynxtllr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nwiomcjo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ixitcjwb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hnlzqoso.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2deuyazwl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2iqpesnja.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zimzowkc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2smjfbrsp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lpuxcqfh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gcgpzjkk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2knbgncfx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ybngdfhz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lfhugipz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cxfwqgdg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tekypbrh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2donzbrsk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xorekrbx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zxiznhkz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2yujldlwy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxotbofb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2stiomtvr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eivewrlq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zxlxvgew.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lckxcrta.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jogkddbh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bpauefxn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2eqnqkrlj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nhtzzvqk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qhpweugp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gsemlhgr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qzerijjp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2idbgkbfv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vxheshfp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pjzyevav.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hgjxqaui.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jdzijtbf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yofxpaca.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ncsoscdh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fwkmjhcc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2drvgdfie.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hilsqrmt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nqpibawn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnpfuzjn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2znelxsjx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zeynajgs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2caluoouh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftndtrfs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gqndurye.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2icxznfti.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2btzkiead.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bmkrljvu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bjzqwlhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tawogxsr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rsdrcyxc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2doymyboj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2azkgenwa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2recnooil.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxbzjghd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ohdxaehb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tztddkwg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lbccuyrl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zouifoig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojqhkqjz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ykvxkeqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpctqzlz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2urjcgxxm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2unekrxhe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bdyqbvnv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mhebwuin.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vyvvaqrf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2eyvcmewr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qxjwnvzs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ivmgaikl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ososuvsl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yclpucjj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdeuwerf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sblqpfjm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bypltzpn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2csqpblmy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2attwspdr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2falrglww.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ixawywxc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tmclkiea.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2cwvvukah.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2btpxdeer.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vrqhemsy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ldvulamr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vmaesqpp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vhlylwrs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2agvehkxh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xtlwpsuk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ezdoemjb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vrfvqjxf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2begxtrzj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vldjmxnx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zhjzxbfq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wzgwxsse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nafkssde.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivibzayt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvthabqv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2uhjjacir.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oxrudeuv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cndyqqpq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhqscrlw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nklnsihh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rvxkbgew.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2swkdsvmt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pauabyyo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fmaspxad.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pluumjtz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lwclzihq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2csfqrdau.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hexaveom.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2iiqvopne.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jgklqqhx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2obmkfrqf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hnbfbgbr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikikroct.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2krdlzxhf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujrqrwcg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2uozxmwtg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wjefqjoj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nqysolnz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cqwomswu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jfuehcpb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lpubbriy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2afvgumhu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnyjfips.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vmbezade.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ruanqlgs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ronhftry.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnxgmii.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ugnfzqnn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwobtcga.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wwlwabor.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kjckktlj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kjojudos.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2abkhqhlz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jsigfjic.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qzocrnpj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wetslikj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zbekznct.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tljoffxw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2huzjjhsf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dgpyryfv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vheujkrm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dcwxjpja.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rybvmrgy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2afwditjr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ygpxihjg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vylwpvms.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jsvmfewa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nvealebj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvemknkq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ylxjjjbj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkjlxh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ttcwpiad.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ngswhkdl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rakpibhg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nbqawjqe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bvnzsjfb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rbatafgi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ogoaauzb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jichutni.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kwexfzfs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fltkjpzq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2egfusohp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jggoslbd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2oikciowq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dxwucbyg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pemctumx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2imcwkbre.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mfhimxfm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hderyxcc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2axbiubbw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cjoznqgr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbmjkqzm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tndgnpku.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2slfzxcfk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cicgaysc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2huvrzjbo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hbopdysl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pouhxiqb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hznxiczs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qonsqdas.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hzgbbcnd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kzcxmzrb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2iogczuvn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lqzynaxl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jzdzjmuy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vsoadwsa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oquyhdqk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2izooogep.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bchryjsz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2scdwmfza.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hfodxzbf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rzruvhgj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxuigvk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yigrcnam.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2edfhipxq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fhhopnli.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wyretvnc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ntchxqnn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mxnpycyf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ykmmclid.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kbrlfzjp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vjuaqcsr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kwmqjkgj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yzdnycpd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vuhqpucl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xeqejxyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vlebuncn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2agklfzzi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2glgzccrz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bgvbmeyc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ssabdmvg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kjosbwuf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zylkwcfg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wplvbbjb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ghepyryf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2drsrucio.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pmhmoysd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pmqufodi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mbmrltil.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hpxgryim.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlgvdesu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zqxungcp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wahyffaz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrzkps.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lajpvaho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzkqnsyd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xuggresa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdgrczdq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xermqxoj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hoocriek.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fzffhsqb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ejokdfmk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2krbqznhj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2chzqfvtk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dphafdla.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ftqsqtsw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2avcaivdf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dfuryiui.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jflqzqqe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2giwzxuau.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lnnxpwof.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kxhnbnfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jvsrzkow.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wmmqblxh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hrpypflq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2iiggihuq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2krkefeez.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bvpervpt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pzjzjqhs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2udeoceyx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ggtbrrxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wtebxbvj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlfgjp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hizpwlod.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gqxomsaz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2obrrwmag.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lrcnubua.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2aymbilbl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2silqiyui.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rqxmmioo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2coyitwsg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ewbujhpe.html


<!-- 参考信息 -->