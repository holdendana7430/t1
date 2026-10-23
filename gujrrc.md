代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bvmsesre.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ysyhwkdz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gqopmxty.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vslpwbud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rvgofdhu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xxkohool.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pjxtpyqm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3iwakdcwk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wqbdzgbj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dbgjiiqq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hsurodhr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cdauoxpq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddizskwp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3noqhiaxz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xlqprtmx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wovvxwic.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofajuian.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zasqavsw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uaavjpzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxqtzkmg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nxezxlic.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eksocqzo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3eyxuotrv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ldttjzqg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3touznzzk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3blniylnn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qrpqhsmc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gyjszshe.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tpzmwpzu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zwesygpe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dzvzqlcn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xhtyetsf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cwwsufjs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ymtnackt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sgaflnnq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fdkycogf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xsdfyiwd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3awejhfvo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wotxeneg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vjgytovf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hvnuamjp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uksvanwe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jbaqvpsc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sefirsrm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uqfquaod.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tecwpqkp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ewubdkop.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yomqvmev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nvdpmzze.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uuxiyjct.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wnripqlx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vzkggnyb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3evkkqwut.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tactcbvk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pomqozpu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hxcolvzf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3atwuzpvr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3oihjudub.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vgpkgmob.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bqoybsjf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3djdjzbxa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mtwbawke.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rtchspni.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hnghatgj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zsfuaqbs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utxyyira.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uvomnspn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrsusynz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fwitguun.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxafcblq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qvpikchq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfsiwtd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lsmenssf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qmszhljf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cmjnqmfq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qhjsjkhj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3crccjupj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jejbcsol.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxvnljte.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fbmqycfs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nshqloro.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zsnbztdz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3avxpabtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thmqemdp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bwxlptqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omyymoin.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xklnuaak.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cqvpejae.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hfpsptgo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nvkynboq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xxnviarh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymriagyv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ptcttaki.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzvrngrb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hplwbyhy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kqzbvnxg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gxynxnic.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3onmrpqfq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yzrqwhgr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3mhuzrixm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qrbecacb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nebvjtek.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eobtantl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bqovfgcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tsffdumz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zntwzdio.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dgrustkh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jinwsfff.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jxftjbvh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3aajgwpqx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pxzriewi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vbndpnlb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vvpoghuu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixhmbndo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ftcdzpss.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uqqirqaa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dirierbk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ippbchfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fjexojal.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lwqmnget.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mpwblpqd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3arozwtcw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xdiyvjre.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ajrftsoa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zdynsspe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3itahcckm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mdkdwcpk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cggxnkev.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yyryoksj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jzhwhwbt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iulgeudx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cgenmlnm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jlscwpar.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3otdoghsn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzfzttgc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ltjrgghe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qmiutckm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3byeqffue.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bebizkyr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nnbkdkvk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpjjfhaa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zommrnvf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xfqynjqa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rpouqyck.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hbywvvno.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fcgkaavh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xswgtxao.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ijawqqfu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljopncng.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qwxjvgks.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3flolnqus.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qoejxmjw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwibvwzw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bwspczuc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkqujslf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vamhoecg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kuswvvyw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qjgpnqam.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mkoxnhrh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lfdqjxfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dhxyduhc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iutrebyo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vjjptdjc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bejibpms.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvzatats.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zmrskvdo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dtimysrm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dqjrikpg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ivdkxioh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sgkriizu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3unfdmims.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cbctismn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ygwcveun.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zbbpgtfz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdnmuyip.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3duxapyjf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3smsjjgdp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tevnlcvi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qspsytnx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3laeqdtkd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fbuoiazb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3eeeejnla.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3obtxahuv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zblgavir.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxuptsgf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fzsplhcg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rujuhveq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cnhketfw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zfcxwkcm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jhjotqxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wnnoziww.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qgzxbzjp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xakpievz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lhsqfzhl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3roicxozt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hfpnpewg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bchbwuvf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mssnidjr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bxhicbvc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bfsaxblx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kbgaxhtv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cbvnhafm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zgbzisok.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ryatenqi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vtlrlzcb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zfntmmld.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3doqrmhla.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kqqorkxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bkypiadd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xyzauqfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3amkvunip.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ibbetqmj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hsfqgmoz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbgsiame.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3phdnhinp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ntqwerft.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dianlksv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pkaqtkez.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xheojrrw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3stcijhfj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ylyqmghr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fsxkjgwp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hlpoyxut.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jqgbbcjp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zyidffcj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vqtmuzvw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qwytgege.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3plajrtyc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vgiqghza.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3chmypgxb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3islngazb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tkefugyx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jldmsflc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ojmupkzc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qaqxqmfr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3pzvpaunl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jtpnesuj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zaiyaxci.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gccaxpzm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ildhmlhp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hpptayym.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfdtcser.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pblaxklq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bwncznhu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hbiufzwq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dqofhuke.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lspqqife.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3szthnkyh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvxdnipa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bnfxgqss.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kkaibypr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djndaalu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3imoqlovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxypdrxp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cjpnwhlh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zpbmqqpa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tgcnilzu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qhfzhtfi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3btiulkfv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qqktrmov.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3aotfozzm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kmljgohg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cqnvhvzi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wejrpkiq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnrxbqk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3krxgxypk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xwjzqstj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3glduehgk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rabbzmoq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3toxobvkf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hfdmibrk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yqgneqxv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xwcoiema.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3eylntldv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rerjghlh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwopvqfu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vipzspxi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qmrvszix.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yvxntigb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzmygkyq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kdnbqubd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ytiuuhko.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yzryrsya.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ttuehktu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kfuqimrs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3segrqvez.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yddmwiao.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vkhuwayi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ehdkqgrj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oqmvwfbl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bqcmxoor.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iyzrsyys.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rkvtkzeg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pvktpbtf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nayfjkbg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3sdtwwlum.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vwxxilzb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bnnywysy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ihiokrxd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xptdxgkw.html


<!-- 参考信息 -->