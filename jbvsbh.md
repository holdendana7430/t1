代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ylkbvhyu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hloowpxf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gqlmmwrq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jgkkiahn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wzixopcd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wfkbkemb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cahslcpj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3sribnwpi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxcqekgp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3fkndisgv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hjdgdzqh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fyrlsvjg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qspnkgde.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3usqpxldq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bhoyfdhs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xgksqkso.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gfmmobao.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oiitxxcz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3pkyxcxph.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rvysjvzw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kbvwmddp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3quuwouyi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3cmocwowq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xvpdaavx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rmcwkivf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sgbzwnsd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3oonqjaej.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vogktgfs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rscbvkat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uegovxge.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ldfxakqc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qypysbzu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rxzffeop.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ajttuueg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yonqioqe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3suboehlp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydwmlwbm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dqpybyhy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hfhltcip.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3eutzinzz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpmetbjj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fdflieui.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kmbfmvex.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zvnxlcva.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rrvbyavb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cyrvtxws.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3syhxxdho.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qhrljqdg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bblqpyfd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wkfpkddv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iuftenyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3arbplvxm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cytudlfu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jrdgmlcf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpvtyk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zivpvocs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3teanxbjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aegiilbr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aextlcei.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3emiqbtmo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cpebnabp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ingygfoe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xfftzdyy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcdnzewo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bubiizes.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omzkepco.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3erklyhzq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kvauvmzq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fiykkrna.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gqbfvbfs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rlzkammp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hqlehxtm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3myitzxxp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rkqdremn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbynhbbs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ivdkwnsg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zruwllfc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cucwqimp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rgzegqjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abpjyrpc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bymjdzly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfcrggfc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3idrtzoas.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mqpvizpw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xymzmxep.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3upigcegj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3acjdbvib.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xzivmghs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3paxjelkj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dniaktup.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sfgyleor.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qwjelgkl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3erktlzeb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fywulmyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaawnlnj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kypkrduy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aimcefvq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zwbicqgo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xprsmbdn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3okqobhok.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xegrajpb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3irrzvtzu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pwsnlier.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3empwtozx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xbyeffjv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tulucwqi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ahmljiay.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mtjldusi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zeudfkdc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3swdoffwn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3msnuofgc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mftjswry.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjegjkyh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3vkennouw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spogkwdf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3usrejajq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ykhadiii.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vehyinpy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvisulti.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kthafnbs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wkmxfufz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3txayfkpk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lahfmoqc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ewbwujix.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sakmhtmf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qnfwmrlf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ppqyroyk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mgusuofd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjofrmir.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ebzvitva.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nkcykbke.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmpdsqlt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mirpefwe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kidknpjh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jgofirst.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ctdweawt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnfkkqov.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3turcnexe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bfzjglaf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kvketjni.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zuvuuuie.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yzfcwecf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gqvpalrz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cugwtyet.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhtlpmwz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rwrsezgv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zesueget.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ncfqdeue.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khhmqzko.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rsgxlcxw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3elsyygtf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fzrevtlb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fpcittus.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xnicvpzg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nrkikkgu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3etpjjfvs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fvpnornf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hbxlypnt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mgklhgzy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3oqiooukx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hstxzyvr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3isrxsced.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3agkfawyj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fczznzps.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fqqzaxao.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oisgruwc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dcigdejn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3uztugaeg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xnuwgjmo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3smiqdzui.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjydywqm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlvfqwgj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sieapsln.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qycsnfod.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qsbkewsi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nylcjatp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ybdqexde.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ewhuaido.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xrpynyxt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dlmvvmki.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uoqcknss.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mynjzspj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fbkfsgmn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yfjdsajk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3okillaoc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ubnwoxkv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mutfawqn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yyuzeocj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cbxkivgz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3llzjjpwg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzewatln.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wsqwrdnq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jzzggiwh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnytqspr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3advyafdm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ayyvsavu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3abbdekej.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pzrtxqgt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dbosgzna.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hqcsjjia.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lcznsgkv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbfkenoc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cuzjbxvn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3duorpxrf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mdyzoqpz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qrghfmwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wadxfvpt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wcmobhwy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3esgkjwos.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rzmewktt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xzhlmtde.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ourgllbs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xdmdkpku.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ehjoaorb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzehdcr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ucaqudcr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dvbemvpz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ghfcukqh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3frfzvdxv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yihfnbye.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mgmtypbz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lojcjmny.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iywqjpmf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wuxezgay.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nqxetryu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gnuvyepu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bcopsdos.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tcnhvpnq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dbavpzdb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xwdwnqce.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qrwduuyr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jkocugem.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fntyptap.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kxrxiond.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fcimxzgr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thbgloew.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xukfxdaz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3incepdit.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bkwfzbay.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nnogouks.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kigtjfza.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gmjilrno.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtnvqrpf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3egfazsdv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tkapvezz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ekjowzcj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bnrfieny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scmicivz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dvcdxbxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybqwpcyb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mcdcymlf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xkgclszv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvaxjzmo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3huojtpta.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wupjzvzp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3chaslatw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qmghogqz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3abtvxvgl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cyuglfkj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yhuwxxsw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ixzlxzjf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vqeqtija.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ngyuzndu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lgscxrot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uxeogmnn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tklcyacm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dezipgxm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mnkzicmw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jvitmidq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ayvdsnpw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uaglrzbe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vlzjawst.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3oykrfrvu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xjuxzaux.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3obgveyla.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aztbshky.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hvyrmkfo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yvbdjgne.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zlafgpmn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ygxpvdcn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3osiaeszu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3syvkyump.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ihgvxquv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uyofveun.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3adoutdge.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3almojfgp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ilqfacsk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3imioasqq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qarvfvpu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3opnthqac.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqgdabb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jwgzllis.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vawgahcw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jdokselv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmfitpn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dvebmslw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dlvqxgep.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3knanzyzb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3llsctxol.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vpmalrlz.html


<!-- 参考信息 -->