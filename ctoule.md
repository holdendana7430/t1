代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3axyvarbi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qdgoomgq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ibteqnqf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jlqiurqv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pfdrptwx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pvkyidfb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yxncgzlc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3puteptdw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qiwbhovl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tmvfipke.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wpvqypss.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qemakepz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ryfwcqli.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fosllidy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3enhmfydp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fshsdtkq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dpgnpvpm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qruhmoqa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vyqytkyf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pswycfuu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3aseoybhq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mzlqumuv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qsrlwzrl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dfygdcrh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mhvzlsev.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jbtjwsrc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3surcwosm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fzslhuja.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3etshjvin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3twpmfzkc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uvzitdux.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3roxwmmxm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3aafmitnz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tdosfkyb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qglhxlly.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lojtizkj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hnnlzzem.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bbhzaoxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ohjyhbjb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3twqlpnwj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wovjbhal.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ynmelwib.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lenkfnzf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ivihhvem.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kxfsenql.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sejbtuci.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rvoynunr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vcrlqoeg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dlrdccsu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kipkrahd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nodubamv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nwxgnmyb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bxszuurg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xgyhrfdd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pzwwzejv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ckxqrzzk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3skhtnirn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukesvopy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yodfoase.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjkditwo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qpnvuifs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awndxngr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gcaufumg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfefxwgp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3oeblqdmf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3givcuwqp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3osqoodjw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3akfbifss.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3upoizvny.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kwextcsz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lqribsvz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wokbfwdl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bpbunsvh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3djyltoye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uihtjqdf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gbahugac.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3agbfhpka.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jkcbpwss.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3piorykfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oykngvpk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3svajfmkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpdeqltu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3poutstwp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3iqwpdcmv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qzuyrrhv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kxflxtzi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3chhenykk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hojfuywm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3udplnhyr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gerktvff.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3owbwqqua.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xicvdmmk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ybaludtf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yjppetel.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tqttdkfc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ebvrcwpk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vyliwoxr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3igbjkcea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rrknbgde.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kkwqzjku.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpjbmeje.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hybekgkc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mqoaunyh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tphqxvpx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jdvlcdku.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wjicglol.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ijkvwbhv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cbtnfzre.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3svbsvdmb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nkwraqes.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spohhbpq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kfsrtprk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yqfzmrvq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tqsgotkw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvnkrycf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vmscjasz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3savjzljv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jecegzka.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pyfhxqzw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3typfdiaw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ostxlawn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yqgjdgqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3twkfqvts.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3snujezkl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fqqtifoe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3etutuuyh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zwxmskyc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fgkhibxb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vvljjobe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gswttmca.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vnetcliv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eteivjgl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jogjbpsn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ldneipyq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbtoqkvt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qpnchngd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qfsagdit.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3umnyidgw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uazjwbea.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jnqkdyiy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ueccvhak.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zbskikvw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eutiiyzx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cflpdkny.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rtuuyorz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oqidebke.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gcghhmic.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fyhufmol.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xezpvphx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3jfhabvjf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gpnnmzwc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kcvtagxl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lsoymjyc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qsaqxmal.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wbgdyilr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oovwrpei.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bwyikcmu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tcazqfyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3agbejtto.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nmbcstir.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3exuznqqd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zdxdtlrf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hglntruh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3knygujjb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gcnwqhje.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bgoivesc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jmnumqkn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gcojjdmg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jbmddlxj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3eflxsmxg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oatkxbft.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3teeqwmtv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3laiwwndd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3csrdpgof.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pgkvavuf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cagiqghi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3crkrvavz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3iipunlrm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3njjbmepc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gzyoqube.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lruqlgod.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jiqbkeeu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vylwpzvn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nilbqska.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ogvrrmhc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3viwyfejb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zagxmgln.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3vfvscfxw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3awjffety.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3czvfrjxu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3paqojkpb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uhiqpaoj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqxhej.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ihlbxinu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hjfdwaxj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bgrkwchw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rdqcntgv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iyuwbetc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3njbyuzwd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ubvopbmm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mkdmrvjj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3stulydkd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ypoqtstu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3axzqcidy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3jtmkffqt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3togqwjbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ygyasrve.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qflbwvvb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jkstgjae.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yshaobkz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ilamqpaj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lkstaigh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dukankpo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rpoiegmw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gqierdsj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3roqumztq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3svuojtnh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pbrfvucl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3torascqw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ntrajigf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hdsxjqee.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wwaturyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nkxuudni.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fiftewgq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kmqrcczu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rvuowzov.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qgxjwdnw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uwnmcxiu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zyghimpi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3owvzpemu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3enecixft.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dyuejlvq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3mqpsvkiv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eaisidas.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vxqejrid.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrhplmyj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qlopbgae.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3atjwdbpv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tzolemjv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qlyqewsm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ycvhovrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ncyuyjxd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3drvbrcdz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3eicqfkua.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ftcufgqr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xqgczyxh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zuixxgwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynwcuwai.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iwaxogvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjdhwlbo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jgvngxtw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gstseuwv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3olpvxqeq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wxzgtfie.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dxaoqvhq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gteyftwb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vtgidalr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dqphcfhv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zubjlnki.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbichclh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfixgwzq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xbuknlkd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3siushfuc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ciqrbzph.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3udjmwzmg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pwryllqx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3genugtvy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ouuvhywe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3knxztopf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3evrzptzt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3iqkorxwf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3otosvkvw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vijwhwir.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rexjmbhl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzchkq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kosnutnu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lrtgfyfz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ugofevxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ffsbbxmb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pfzdxbjs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mjurgajw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cgcazgez.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3svxacjyl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xyyzuukb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mvfdpkqt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yvyucsxl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hlrjjibw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ssgbfvrp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uhkzkdhs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ypacuxjn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nalobotc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rsfbzeqg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqkatvmm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qsqsnvab.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yimnkrxf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3icqsasqr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hntipkse.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3awrqrnfz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3apvusvxi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mjqhchrj.html


<!-- 参考信息 -->