代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bmmsqmmw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cjzpcrnk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ncmmcxvh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mrkkhawj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3enjgdgmw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mckoeeyu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3orzhmibn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wjssooax.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oomrzyuy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dfkotrqa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vkhnzblw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hoiizfdo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gousgwll.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ufwmtmbb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mokascnh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bautihal.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3olduxchj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuegkoku.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3banfwjxa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tnnlfprn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rthczjgj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3djnzufoc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oyazxwjf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3imvutzvo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3iufnkets.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3disdgdly.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bgipizad.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3abcsklsl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mkdaknyl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3luozjdvw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3aboktylq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qiqqauab.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sulupltj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3knagsuhd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iusblshw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rpjjilea.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3exntgyry.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ajefwobk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wemxdgcd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qdcdrnpt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfftkosl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sjofwqtm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3huqndxoi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qijeeuxq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nkxxflvv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mnmwzfmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dhomoder.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3goxbymlt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ryakssgc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3findukhm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ipyqxyew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pprsxwrr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nloccfef.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fgkkcfse.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3msffwwvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oiakdxte.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wbkocjda.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbvoywyr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zyiywdtr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvdvzoub.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pncmqbif.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfcempcn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dtykdjae.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vabwmadu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pcgbnmqt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkaswdvh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wpvartal.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qgmdlyrc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3oqppqeqv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xwffkjhu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pjykakxz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rsykicgj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3shtmtoxm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3aazkxazs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3meoodscp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sjlwceuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qhgwztec.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3iwyyfjxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jerwshux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgkkwnqt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3eavzpwbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vydqwyct.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rzmhbget.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3obovitys.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ohgfwwtg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hamkecht.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yfrzvuli.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kybixigh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3eccupgme.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zywhqsva.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nkjcccdl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mwycqjvv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3esngvsgb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eosvnjfv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pflngtme.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3mtujgjax.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3odjrjyka.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rxoibzqx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dsxnntxg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3idowydeq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wxikleuz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aiphusjz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tejccnfp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lgvdeqzm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3veiasqrz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gkdcveno.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vzficmqx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hdfnrnrl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rqazxotz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mneaiprw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nejcidhf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3drmmdsxv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqeffmxl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ydrvpbcz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fhvphtee.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfwqpden.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evgjfzyf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yqdaossk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wqyzjeel.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3arhpzsna.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjtcuqej.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mknqmzyr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qrokreyb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dwrcnrns.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnssdwec.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qqllzgfc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3strnglpf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3odtfbavw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3emctsgkw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vebljuim.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zufrckiv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mbakhvfw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jepetudx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3efyubeny.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gwfrhbfw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qjkdewgz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3otbzzwvh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3oofpfdpj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3famdpsqp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3urrlxrpm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qefxmhnf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fbzsvxfn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3acciuuqu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3olpryhjd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iqrulmhz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3btimkgoc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wtiecibt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtuqntda.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysvkpbwr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yuvhsygs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nkkksdvf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zkudauno.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3abeytxhx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ndzzohjc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pqezehml.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iatuesbi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gwoiheqj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xkuynxeb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ejcymkrm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lmvgqtzz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxbyrfh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ccihlraw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pfgeyfvf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xiravggm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yjdvdmyv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3icjypjaj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ubbfrpva.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wbmqyjxp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bvwabqan.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3txldstkb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mppjqpxm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjtuhzam.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ixrsqkbq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3aglojiro.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nzjmzpfl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cijetkhy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ztizqrbe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3smmfgzcq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zjgmeoth.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3meydvsco.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3frrupiqn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ypdfqozh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rcgvkmnv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ugtjjuaz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3emqnmbdt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zsvkbzpl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tnkgosfk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3scfytktn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3juzbckzh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rtxhwkvu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tghpckzq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bwtvhixb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ilaiwusg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3herkjkth.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3usyafpqs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xgagzciz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fpvyzeoa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hhutyvmi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3otvzbucg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ucwxzigi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ufgxjxrt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3patczfws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gkaenvde.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wxnrulzn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3detufewd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3glxdtusd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hghjwidw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3khnkidbd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3anyvibqd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ytjhidbw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3skspzttp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bpnygmnt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gtgckfrg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pukknfhe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3aiirxrzf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zatthxzj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mpdjynqi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jahplgbb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rnmmrwiw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rzysnhxc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpxvlg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uzsfowqj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3flrphzwk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nhitdwle.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fdoilgnv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lemzrzet.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3toyrtjqe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3umasbfvv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bfcyhnns.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3khalpxmw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jiultpts.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cjjzopiq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yedhboob.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rjjwpzek.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dwhoxsti.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxrlnhyn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dhrygsyn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccjbjbwl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iuwqzfws.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vdvvdwtd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3incgqchu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3aosuldhw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3htlmjvam.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tedtqfnq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zgvluxqc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qqhvvfop.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hiydvosx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwthlxjo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eosadnwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgzkijus.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3frdezqeo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3urcnebhu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iyrzveuj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qgmlfkht.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oakeovjh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jbyflqss.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oncnhuio.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ihudelor.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hfqgyurd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3veicxtyj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jshuonyw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dropnzxy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dhfxsxkf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ayytqtmt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qpniywgu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gggjujrw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3skmbjtss.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dymgsmls.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wmmlblor.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pvdqvhke.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rtplvhjs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uczpbjyt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iqqhydlf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3omjwuydg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lawngpnj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wdlcopqb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lujtyqmc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nchtkwru.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gfoxotsi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vthcwxbc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ugvrayou.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgzxxhfo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vxyczaaz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zmwxkyzv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ccbtrbvc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wnbbsqke.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qcjubhoq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aebhhwet.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3afrfcthz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ibuieepx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mhztrovk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3sjqbbafs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fpumpxhh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3arqrjkoq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pznkiqft.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kmjggsaf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3optnrfeh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pxekwtje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ewmwyfas.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lmebrwit.html


<!-- 参考信息 -->