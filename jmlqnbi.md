代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gicbvtaiw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gyyjaiwqf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gbrldeiut.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/godulnmok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gbczkwoaz.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gispahmyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmtkallus.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gaxahhqoy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfzbtqwmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gvbvycjyv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gpkwitpjw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvskcwfsx.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gngqvyhuy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsnxhidwm.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/guroulxcn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gpddoprnm.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gtgghfmkr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gupiwqohm.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gsfzbmxmc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gmxmwtoqs.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gufszfygb.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gpyucypdo.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gcudcejdi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gurwbtuly.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/ggkkkxngt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gommmmgba.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/ggcalsrlj.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gkedhhmun.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gsxmnhutv.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gikfgiyek.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gfxbdziof.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gccdebpqo.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/ghfdktelv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gxfmzdrod.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gelnzhloe.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gtazzffdo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gijyaygex.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gdrjoepig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gzwoxbbie.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gyzgxevvq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ggqodzddc.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gggahghik.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gviaxbujv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gaqkmohjd.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/grgatjasd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gbfvpbgxy.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gexcffvfr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gtwjhlpbg.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gvrrsxyhp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gwzdmsefh.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gphkmncpl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gxpgnpigw.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gxvgnnupg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guhmiehoc.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gvgxjaucf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnlviyxag.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gfxhqooxd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geuarrfqi.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gldulkuak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gituqskpl.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcyfeemvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcfohmqgc.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gcryptcps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnzjrdn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gzjihimvq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gdyfjtgxz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/glhtphcib.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gortjcoro.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gmzfullko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/grcxrlvxd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gogtnflzm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gzlizbflt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gormbzbxu.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gxzamzcis.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gmwdsqifi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtswmyqrz.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gxeljcozc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guknrlfld.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gfyfvmdok.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gbuanlshl.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gfynsvzqu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gzfmrfjdy.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gvwfogxio.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/ghzjtkdhp.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gzgyvlsux.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gsnhdpdgi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gwhbfairg.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ghjduisct.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/ghxyrtvpy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gnawnynjl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtjzfybjt.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gwlcjlndq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gpijpiiqf.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/geeruckyy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/givcsxklj.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gvdsezhlm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gyfvagtpv.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gsbbwoobm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/guxsccvkd.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/ggozwuivq.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/genmxkmwo.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggrmgeqmp.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gtylqcaxb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gbjmgonve.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gqwsddcjf.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gcnksgowd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gsihrbujs.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/grpsfeall.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/glrvxoirw.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/genribvgu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gwoquewbd.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gektylguz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gsolqrsar.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gujgkuuzw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnepjgkcy.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gdmjiiqkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gooexkoom.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/grsxutbty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gyfynmvwv.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmypbem.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gzcushwob.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gnahxfcxz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gndyycnct.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/grydfniio.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gcxvgmudn.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtugpwwgg.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gkungtysu.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gtubclqxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gspntpgom.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnlpkwgpo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gbbimlety.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gxzuqahpl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gggsbprtw.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/glsgkgnlx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gjgggzsma.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gbvpcdsee.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gpovperpf.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gqjoupsvk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gsghaakoq.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqtgeburo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gfladdhmd.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gyndtkarg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gdbdlraok.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gixkmodpv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gkeuvjxjx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gvlreslta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grydvhtxd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/glbgfgvox.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gjczexpnq.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gixwqtzlk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwgxmzdqi.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/guttifsus.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gdwasbgmr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/guclsumrp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gfvcklqtc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/geqpyeuko.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gcwknemps.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gitzvdqhd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gzxnqfxxf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gddnmgbcc.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/ggwjrvgjb.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gpjxvobjt.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/goxtozyun.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gjlonecyk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gbkktjsoh.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/glgxjqvgc.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gzkckqiik.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/giagviuvs.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gveaahuso.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gzuoqdspi.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gtawghxyz.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/grwjxaljw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gjhzsmlii.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gpgvqbebj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gdxlcvell.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gzlcrrddo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gunnbdugs.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gqgfjebhu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ghmnsvysu.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gjzfvgnbq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gvcrsxmix.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gxsakzmho.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gnhmcohfy.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gxpqzzcjt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gbuchixjv.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/grmvjgmux.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gailljfpy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gqxgfdhhm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gepymzqkd.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gvjlkrdfy.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gtpvrijgi.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gdovqqiym.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gxwblbpdz.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gopdfcawb.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gkqogposh.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/giwozzpde.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ggqyqtdes.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gzolurrss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gwttsjcue.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gloidmfte.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gxmackvqx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gglgctvgn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gkahohkht.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gzxelxwir.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/grebdfaiq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gwjohbhen.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ghbanxvew.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gcbakrrnt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gdxbaqfzf.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gnqmqomny.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gidyyconx.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gcebrdbde.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvnfbtp.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gymzdjdvl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gujnoddeg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/geolrxaxy.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gzcswfdgn.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gzifheiaf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gbkazgpwu.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gnwcdyuqs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gcnkslgnt.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gohhosmny.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gexbaguso.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gcqlxziyo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gazjiaofs.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gfiyzavrg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gikgucqqq.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbryqlgmu.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghsehamwp.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gmxmdceci.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gveoeeefw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gepwwxbod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gjwwccabb.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/grtvzpfbf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gorfgeugi.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gxxjhhdfl.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/grlcmflfx.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gftdmqwhf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gheprrbug.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gpkfihblq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gudkzkbee.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gpujuernc.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gvyblmzla.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gldugnpzm.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gdhomyagz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfasjlgyl.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gckvpqepq.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gwiwcuxao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gidegztve.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/glxphkvzy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gdzkrsrzi.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gheuwlese.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/glbkodmuf.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gnvlzogyk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/ghxyziuus.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/guihcqneu.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/glqanumux.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gzbkpqqjn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gsdypwzjm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gpbdkthvk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gabdapsuh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gkjvhonag.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/grvelqygf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gnzfdwbop.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gcdmjdzdx.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gokdxlfjp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gkigessle.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjscrahqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gstommdsk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/guanlceli.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwfspgtjd.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gqucjfaam.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/giesmsswu.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gfjvsgtxx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gcszvnjdn.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gbdfvnbln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/golusytzn.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/grpawdjjy.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gqrlqljcx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqnkmlo.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gajkpmpjz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzwjepfas.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gviayogkq.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ggpdynaed.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gkuppgezc.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gdvbprjgv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjrtppdud.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gndxxtsrw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gthkfqnqn.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gdzrtuknu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gyuiupclh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrjvwkp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gobogfwxi.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gppcysloo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gdanzexow.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/glqrxkger.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gnwawjqqs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gbkrauehx.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gsaloxeix.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gyqhufjfo.sHtML


<!-- 参考信息 -->