代发 wailian999

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdguemket.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwisdfbcw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtsrldgd.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/grroufdgq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnhvrbmu.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqkuhhpb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giywezslw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrdrtgbw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gusaiapao.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnugfnmf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqyizwc.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gfenfiqhd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gnxxccrij.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/ghygsrveq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gndqfswoc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiekupuu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpacxyqm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/goabydzao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdvjmuac.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/ganzqnavw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvfgzywz.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwswbtxko.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfykndvw.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gzvtekjov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gijhcabrj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gcgoxhikk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxfotzrb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvozjsofe.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuflxfcp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjchxqekx.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/genplzgyi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/glhajvoxs.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gczpvxkyf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gbffxpcrq.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnqaoxwa.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/goyuqhqbv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpxenkuq.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvyqebsw.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gpuzltqrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzwogjjr.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/geolglzzx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gyltrnnio.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gedhbpcoo.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/goedplmjq.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzszpnncs.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnouobvug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gdakcerci.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxechzqmr.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpzmrtdz.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gfhjuuods.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcwxjxpp.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqhnjkpg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxegsqpxz.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gemfcchmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbynocrcp.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gblhkxigr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfgrplb.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtimymfzv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzilujsm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gyjtftjxk.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/givcoigah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryhiljbu.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtodknea.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gkbmpfwrw.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmccuhvbp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmmluxoi.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjfzpel.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gijacxogj.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcrwouik.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gseasakoe.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvudcoqji.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmuztdlsp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkbvgwmh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkiucjkp.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gciapghed.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwntrjfba.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gghaxqsmf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjcdcgt.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/glncjvpye.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwetmatt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrkqxfn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqnwixxr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcadrxrqe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikqbgwjt.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gbvqucawb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gvvdjozjm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpbpxplz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudzoayp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gxqcngygg.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gucoyxkfl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gimqizkbc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvatsjewu.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwyahbzq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gowctvcqx.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gytaxpanw.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/glguwgmov.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/ghrvibkpn.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gajwdgqzc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgvaulec.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghssxgoas.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmicvnv.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaoivykx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfiggslp.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/grfswwygp.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjjspqo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggoakpcq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhqnyee.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaixkdzq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkxifjjx.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktlkytl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmeimdsq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gekzoouan.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwidojqxg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwwlfqfr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjgenklu.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/ggldflefh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdsoplep.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gparbbtns.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggynyyirg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grywdmppd.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotfpefu.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrtjjzw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgtwcwmd.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtptzcklg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gokhjgifm.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ggmufmvni.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gypnvojdz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxtgptmy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhytlfde.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdruxcwkb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gholyugcn.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeduzmqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyxtafds.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyymnjghs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoxrefhi.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghvdvujxc.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghoayxjzv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gstiiwqwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqamalwg.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/getnwbvao.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyookwnlc.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gfmskhekd.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkxmuwuh.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdihbwxnc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfaepogqg.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glazwumvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjvbgcpn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuojogpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndacyimx.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjrgkpak.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gqqpbhoei.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmjntcso.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxzuxay.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gkypnxwlx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gagrqtqdp.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyldqxqiy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfdyqiks.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsiccylj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnftkxuu.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihxuddwz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxthscdqj.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gurquepqk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gplvnculy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gifutjxmu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxdpidkk.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gtpgqharr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gemiqcful.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gptueagox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gooadnwem.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsmhngjq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwsgfjwd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiuudwgy.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmoqcxba.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtqvvsw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxnzvqyze.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxabsdpc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaoftlwn.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuluzag.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrtgblz.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/glskhrgcy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkzqvuobp.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghezmoprr.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhrsuzsv.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyxwtfwtj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvkfgwjf.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyiacvla.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gkyilgwfr.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gqqmfhnwk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoxzlvzl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvbprwnh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/glftjtnzb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoepbgwg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvhkshktz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawgaxcgl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmiozgwi.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrttjiwo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genjyfezj.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpjpuhkj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnwtgnnor.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdiiapy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gsjcthnrv.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdqoogwgc.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guyfkbbgs.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiisfdoh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/geshekkvr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gleryszul.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjodqdfmh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxvnduhp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gzkroxzpq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glhrendix.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdfkkrl.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gujhmulvo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlhrwwbw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnxpoxrh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glwsparzp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchxkufn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdrjsmqa.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqegqulic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfiakiiv.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gekruxjro.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxfbbukat.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggacdecub.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegeonzc.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvgjfmvj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxklmjfo.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhbgvdfy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gisrfthed.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtbwdvjyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gnbbeflcj.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqlvtxwu.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmqhilvny.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/givhhgtzx.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxlvsbwn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghlrduktn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghaigncil.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjxoaip.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvmtardg.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gntnrmior.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gmywjkwpd.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gkpaukain.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmyzpdn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgapjbsf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/giblqbvtd.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsezwddwu.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giljnibve.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/guzocvcyd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcvimfvwu.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrvyfuuj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gansbrwet.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gouunsfjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnelrayut.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gntebjvvt.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakcvkcn.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzmomnfr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdmwbbjmd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/guitzsida.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goximwefy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwklvrjbh.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhlhxpfa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveezdujc.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqhsnebtp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goatjzywg.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsoqlskhc.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gbsnnykni.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxfrdlvw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkbsaxqh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpfcillas.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnzhogij.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grmceaonu.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gdogldsev.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gaymoufsc.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grwcrbdkl.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdznnfgu.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gthuvzmqb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtspoirjy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/grhydtrnm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gszomqekd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gaqzzqtgb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjnlmjqb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glhgrfnop.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/grczellks.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeygoyrw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gxzliqkhd.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwarwzaln.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbruwphmk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuqrwghn.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqdkmzb.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcxronnsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glshojpwg.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gaejnmgsn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwzdrqzqc.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/goklfkopk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdpietdk.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdbhicau.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpyzfqdf.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdktosec.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbwiytye.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvrfqnku.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpggzagq.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcjpitos.sHtML


<!-- 参考信息 -->