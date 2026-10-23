代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fomebkfb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bztoyztx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tyuiqfez.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3eaxjzzxb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cuhgqzfv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lryaflvn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gkpmgjlb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wjrpxquw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3upyxxxoq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yhevpruy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hmnqkjnp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zvziqovy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ipaghsqj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fzjhcbvs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xoppoyuy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sabbxuer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ejdsdisf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jyjskgxu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sioduhiz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tlfnlliu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tluehupq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qucqiaqd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lybveohx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yhkbwqcw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3iccclpjt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ndgisngs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hmsqqzdg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3snfsvwwo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mypnqmzv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oihzsdiw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yowqtrot.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vhvuarvc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ebswofds.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pstyvzne.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ahovcrjz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rlrwyvyh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rdnkvnar.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tnxtvsmx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mbiphnvv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lstgtcfy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zpyzmqth.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dthqrmxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3thekqecl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wxdjjtil.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ssmywbmh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3aootmmml.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dxgyqcxw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hwhjlxet.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njmlfpbk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tqgjewwi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xnlcpezh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oapfkgss.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3siisrisf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tmnehvcq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ktmrycza.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3sibekexf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ivwcsgjn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pzrogtrf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ykkssthh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zmppzexx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bagtbirv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ozyhhfbd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3axeayrzs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jibzhdgr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kosoejul.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmbncqqq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jzaabuwu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfqjmdkx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ethkmbmk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tskjujho.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fpdexmvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljwrllms.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cvnpwlgq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgjtgeau.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jconlnby.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3khpaleqc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jmwmqyxq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zkqpldra.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tgxapsep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xgqvtlxg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wkzhufvw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nbqjtjpe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wkfpjqtj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mtbeqdjx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3yjcldyhj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3iqhzjvoh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3plfhzovv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxrsygxv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ayqjdszm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgpvvhvw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jmfuuzog.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qplulwqj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wpuooafw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nauwwpyf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ycexuynr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxcnqpte.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3fqootoxg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eosinfgs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cdevxcfa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vhxbtvxu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qoqymnfa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qqfibtbi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zoapmyti.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3uqirjhhq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dxzwuoqc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nbbmkkrf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hccbeguw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3obnsdwwg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nsyqtpoq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mdzifrkt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3owwteatp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nqlfxkhu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nvmlaujh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qdcyaluy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cjkatocm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kfcgnkuk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nraayeur.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jrxgzdlk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jgwdrlbb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bmhmwbov.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3czhleyep.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3epyrverz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3klnmsinv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iuxisned.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3btzpfyyj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmghhckn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ymorfkyc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3youippbq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3widtpgus.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kjgdtgwe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhfklbkm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hxstxegh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kzlgbutw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qivkcmkp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tuakfjwp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhcuxgyp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlnjiowu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ssltmoac.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3txlaqodb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxuxxezv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lgaznxkt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kzjailen.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yqmtqarv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ftzfpzak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayowyiic.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3htsurnjl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3sbsruiui.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mldibjxw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xqzmibye.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zzvpktdc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mcbvqmpo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxclbsul.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hhvfwnjj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cxvhnzqt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pgmkygix.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zvxbrwdm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tovbfqyl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3otiyzemh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uvccdqwq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3sigfmykc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ogedfivw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gkyzafen.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vwyhehen.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wypcusws.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zzyvfsmx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gafwjrdk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yvthjbzh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fzvnlikz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qbtituzc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3acovvafn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jkoaqree.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3eqeduhjb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xpgjdfry.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qcdsosrk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vxhqbhij.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cakhjogi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eoqvfcpd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yponsjgl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3coywxgcf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkfaiyyb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gtxqkshr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lrxajhdj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mlpwmjvb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ghjwlahj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3acbcihgk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mhtgcwdo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3flouudec.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kvouxcwj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pukvezhz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vpodzupz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3clhylnni.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ikjnvwhr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dzfraseo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3louewmpw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sfocqwsw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cljhzydr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fgexeblo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wgqidohr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqaacpzp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wbgwqlmc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fxcpiwsv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tsitzild.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ruspbbdf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yeeyemsz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yzyhsdbj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hovmavfz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cfpmrroe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kxbymgvi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ndrlrmwj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3swnbvxhe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lsilwzlx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jvkndgue.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dsxdlnwz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zqrocesa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xqkytmkt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gehliqne.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ipepgllz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nfuvheru.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wbhxvgjb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jdwupcem.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3valjctag.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wgtaywbu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjnqekl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kwmlfbgv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tpazhdmf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ifzmdyer.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kwpgulqv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kqtduljz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rznmnxwt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sdcttotz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fseazlcd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sowktixv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qejumxuf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lczqdyqf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ekpewioy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nqajimyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tcdtelra.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ghkpqsrs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rltkutee.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nrdhfhvb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zodozktc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zxnbvybh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lnczqbgo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3malalmxw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bjbvmvqw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mftcjyep.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3foynwldf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wmngnulw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aesafntq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iaufpkly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lulritcf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ysuupckk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gjbrsiae.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nbizlhzm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ktziyudx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bralglcl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wnzlgdse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpeiyekj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfeanlfa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iaegachm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lhqbrcym.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ufuaasqh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bntzsknu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bblkminl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wdsyrcej.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ppymujqi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nqytdxmf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sinowoni.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgfndks.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3odmtjqsq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xeazcrhq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wqqwzxgj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ezfivipx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ksmeodpo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3otsjjzpb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3erxcexfr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ryekbojk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3odkosrqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ggajsppq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3itwuhpgi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ftjspquv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3smhojivr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vrftgsxz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwxjzz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgfuwkw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xveitivg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yzkpbmvf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jzsxlabj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ytrlnfmg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmprxefi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wxmbobwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wqtgumaq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zextqxli.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sgxwigwx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vrupfjmh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ikvsankz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gjwwrrjy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qnuukxmh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lhlewnnd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wzxmgqnn.html


<!-- 参考信息 -->