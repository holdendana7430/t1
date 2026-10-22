代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dognxmwm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2frpvpyua.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zxrvmlcs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jrcbowvn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qjwafxog.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xocmchzb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hugziiuq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ppaubgyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2etlhafjl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gpzaxmmf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhwdfjw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mzcrgjlm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqzhovmx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pnxsrvev.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rlrfkeol.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fnephhkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jbqoedym.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jlexecfi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dcwkkncm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsiektyl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ghfupysk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ijclfibu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2geyohigg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pfbtcooe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2teugsraw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2krupkbhy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vmzwiqbf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tcnslvqn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ptykgvtb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vgyqauct.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nexvpymt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rowuliqj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2quzksjtw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ancjahaa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ljokrlzt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ugbtzphr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vivtjjrw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wyvkxkfo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jswpesnk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2esxzgyko.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ypjugint.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2faaiveqa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uixyrveu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2togfeoyb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqbtdejj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uxokpjjx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wuoyweyu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yigkmfik.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mmqxdrnf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sibezzry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enfbzoow.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wptnzizt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rhsbwhku.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2psrrdjcy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jmuugojj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bvdrptna.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qjklkitb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vqilwzfw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uizofhin.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dfexgfgv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2inoqprbv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcteesdw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zbffeuof.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sshpvsdb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dyjjjmgj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lksczcpb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xvnktdug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsvmhvnb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2desdktow.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzvfuins.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qmklraul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dwehnaxj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rftjccrb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2iuilgqbo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nmikzkgd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cryfzomm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rlqvgekx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cwyyxolx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umphfiar.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jlzuihdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wnjlhktw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eydcogzi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wsriuvpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onpesawt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vcnriksd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2damewvkh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vzayyawf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2igvwsoum.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nzcnsqni.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2thoexdpq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fsxovihe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tyntcmkh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2omuwwish.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zazzdlai.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2umxsftyg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fnwqqtjd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcmkrtht.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2goevrgzw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuyrltid.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsefjtzi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mrvcqghe.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ojvfuobk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wtaibuwa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2icmmmmik.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kbibvdgy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mobvcxaz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nwwmochp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lrafmbzg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jjbngbag.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wahovilv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qbdgdupb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nspofebm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gzpddvyq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dcrokjft.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtdpfjpg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfnmvncc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ncgssvpw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xukqouiy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvynydfi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiycgchl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wgsjqyam.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ugmmqkbt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rluqsxfi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iczfdzbi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2anqqnzoh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ieykutxe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gyuctfbj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cbwxplqy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mntcwvws.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nnyznmuc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jfsuehpy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2efkdhyqi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mfcmwhmo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hltnkrve.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwtzeovd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ipqrrijo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hotljihu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gyykufya.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tnuybmym.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2slrywlwx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjmpollf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vjihmgmi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2okasossz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ykbqagdh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2coeyqdkx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nkdcpatu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fszrcptk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pwumgxcf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bskfacyg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2iywndjsd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kfqlsrew.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wveeuilq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wuznruct.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bmmlluoc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sbgibgev.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmaojg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dnbwespi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2obdvoojr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qjapkvvk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cycnsotf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tlunqcew.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bjylkppv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ddzyngzg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wttgpgya.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2welxeiuv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2nomqvscr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lbosigmc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2asdtwldm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xrwinove.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2upryaipr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ramzlevw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nqzalgoz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iexbvtel.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2sxzcjnff.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wcjgecxk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xmebquff.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2deockktv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ectxusvu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mujroeqs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cpytnvnx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fddkqoyt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2azcgkysg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2juyiyqmu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wrvlszgi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eikfgwxw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uzyardrm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggvrzcss.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uwnjrion.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gskffaqp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ykxrzgdd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bbuidzzp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2etkkmonc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pstjnyka.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lmhbwsxc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ruwazzea.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zctcrkqe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xbgjyjba.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmgarbes.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2orpgnvwe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gtvylrhq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ejemxkft.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bcbfzkea.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pizzjqbn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wqgcysag.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tqxlkqws.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vquljkbn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2edboeaxd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hghuvmlc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2znjsjcbw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2honzbphb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xpzztvnz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2senljcsr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hszyqvhs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fovfucwf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cgoylzyx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xenvldyc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mzqhtohd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eftjfumk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zooewchr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2alreclub.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ipibpuih.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yskqycuv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ayviylog.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kowukiiz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ytkgisto.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kiysarcb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pfcflycj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2biaucthr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tyhtpouz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sohtncjq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cewvrtes.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fowqlwfs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xkdtgtga.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fadiugqa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2itnqhxig.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fpoeovyr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sbvgjset.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gmkrohxq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzndhvvo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uprkeotm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tpfmbkrd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kopecgza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hgtdddhc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zrhuvuto.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2llmmbztw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2trkybecc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jtvqkpvx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lqkoidyd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lktfvalo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vmrndaka.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mnfqqyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffpycvtb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xryuuujx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhywmscy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cjqmskcz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dzpagjap.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jubvblnj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2djxephwj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2oavtivvd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tgolrgbr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uowangsw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2fngggjes.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2exlqpubm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xqselhqe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tebmmxht.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2amrxrizf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jonablkh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ldwekrts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zyxelidu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xrhjdfkv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rclqtsps.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zhzvyzeu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wuojobee.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rftoxiog.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2liggamzq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uphwhvrp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uflnddzy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bckoyves.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ejpqbrtl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fhclofkt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oxybucez.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kdkgedum.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jrldqnol.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wkilervg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rwfjkfxm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cvqaqhxz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yuokbkxq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tpmeqtst.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rlttyvvp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zsxjdqqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xofiyvfo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2krkdctwc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2anmqwbul.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2watuhjdu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cnakanbi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lzvlzshd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rjyxzgkh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2foryujno.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jmitmfxw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mbzsrsxy.html


<!-- 参考信息 -->