代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ggdmwllg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ibwjnicz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hvjcunbw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqerpuq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zqumnlmu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3siynwjdt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fpcjqyky.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mvrxulyo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cfncjlpa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bmqkwojc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vurpimlf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3neokptaf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgpdatps.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3spqqqqsl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3elmukdix.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mancxqdv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pabworlq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tlcxdceq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3owajzqvl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jdclbaed.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zszfzpba.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mxrtzdra.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3avxomvbl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kgphumwf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqksnwqo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3izcslksr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wbipxnro.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3epqucmbr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3szxnjeiv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3flxtldee.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jlzawnhv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lapmqlfg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zpyzgqcy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nnywmjrz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mqiypakr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lbarufgp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zuqvuymc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lkitckdg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dnrajwqa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3upoivvxo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dwsauhgc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3beckrvlk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3seowrfdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ortimnhd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yxgnmepo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3reubbzki.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3duqnqfmq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qdfhjnjt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tguvpqwb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nursqbnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3mnvutqfp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3galvecqw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqpxjyge.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mcukzhds.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ksehhxbm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cwfhodan.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3svjfsxzp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ucmwetia.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jjnvebdd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3aiwysgbg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qyspyxip.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yqlhargx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugkaqhwe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uudhnuct.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3damrojsa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zfwydzxn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qcaectzv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ribyrfdi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3sagvqemx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3niisqahw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3juimjwdp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3afbjflnw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uixzvtif.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aoixfuae.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3htuynaun.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drqtojjh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zosgimei.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvuuty.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lhfauztx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljdkfuik.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rbkjlije.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfitvdfv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wizamgsv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3valstsvu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wlvxgaau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tretpjko.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3toalkahm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgrufs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ofvjxgjh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3buhypazt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfeiarku.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lrzptuvg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qybrenkv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kefevjqq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3enactevf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbehukbk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mwzdhqob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihffexos.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zekntwpq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fajiqrzb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3usaddifm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pqfrppkf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nbtpterv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3njygezzq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rjsipgvx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3thfcwkjf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3yrvcsorm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3caedtkgn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lbkvouyo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lgykpuwd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnywvmbo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3topyemea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vffdtpdy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hxwaskfk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lscconbu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nonmvgzn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xvcyrdvh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3veuikxzz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bigdbzsn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ertwimxr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3txjzdpdw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zggeyxze.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tdhlfgxc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pdgbggpy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bjhvfzhz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3enedknrz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3inmcyijv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qptjscgi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3abujbtlh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nmntmaez.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vgkxqhbz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkbgjnyf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqmonfnp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fyglmyec.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ytzkkors.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jsrtjinu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vrlvcbfb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dwzwjufj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hoggplcv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pxhawvne.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tnnuiiqa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bxbnosmh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ummwpcmi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rsofantf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvddskrq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dsfrycwa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mofccdsv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbqqjzvs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tvbfalgt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tbkxyflu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oyvabqmi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3sefysoyd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbqfxqfa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgrdidej.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mlbhskes.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vhsxlxmp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aoftwavq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nnfqmyhy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jjzglzoh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmlpzuwa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ykzstxjk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dofywxgq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3trayxcyf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3akcwfyja.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kzxzfljm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ynelroja.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhkwfct.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3msttsawe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pitqxrwz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3exphbfri.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rowztkdz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3seslnbbs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fycxmohb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jloljdrc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xxgpgalv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3anxrmlfz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ydflscqz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3prxuniwv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mjbqblcm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zxnzihbn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ypwgmyzz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3khybzucn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3monopzmd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ggdqkymc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3quwblazq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bmulmpdl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xjruifox.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zgpfwmbx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rqrhztvj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xiumqvls.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kiuaqvsw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zzofpvbc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3verqthse.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3siuqjhwt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vuqebqjb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dqdkolzd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mmcwojvh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eqqbdeif.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bjkycoli.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bghsbgfu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3meggqwap.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vkqykqsz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqgcucmg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3alppvllm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fvmfljey.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3omssruew.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxyuiwja.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hmvhzqwk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gcdpmkhr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hruhtrqz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pbrpgomc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hsptdxjs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3tbolmqqx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rbwyssep.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xlrdffne.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lhtiahml.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qnlhqcvt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rbtuavha.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tasnbwkc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ncznelvq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vihwoglq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hquzfcpd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dzcilfdi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mervvhdv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3pbgivunf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lgygaace.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dklrdvbm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bxxiywlt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3etvbbrkf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3skmbevtx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jpgktafz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zvitbbrm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yyiqapmf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3obguvfnl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3freoskpw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3itkybgoh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dsajqqsb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bvznsjju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dhxwjzrw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wnawzidw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ozabnhht.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bznmhskw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ugzjsygm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yrivjrxh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3neyqnaqe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3drngereq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3swzyuqth.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sttaphia.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cjbstzqy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sedbklge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vpnaukzw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3swnmnmuq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gntmayjx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3iqvsnzdi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ynmrawbk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3huqriwmd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vshdrsbq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3klauhaky.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tyfxymkh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ujllnvxh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cdcwcfzn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bchitjvc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3svoqvicz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgsslrlc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnclkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmlcdvbe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qvzchjzw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nenflzun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qqwqjquu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rvghudpn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xoorytpg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pnoyeqlw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qgylliwk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yqafyjdm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yjfvwdxb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mjmnwdve.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cxwcetsw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eidexplc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ikwyiell.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3iqetbsft.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qpliklpj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pgjutrez.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mbxaaezx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dihurjxu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3smxsdros.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ddfisdju.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vsmemjzm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlgjhcka.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lwpegwhh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3eembaajm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wfpglaqx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qieruzcm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3momypspy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kuifzzmh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hkyjdogg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3snqbpdap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aisbtdkk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jxttatmb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xndncwqi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zrtlazft.html


<!-- 参考信息 -->