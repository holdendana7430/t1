代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jjjrexmf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ifnlyoes.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nwapfppa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gfsojemk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vzpsunfx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gbjceszx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2aptizkbu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2glkvlxad.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ghcsuqsm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jqjexzth.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qlyzxwlj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kbvytgrn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eekrayuh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ppxzdvbq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iseooxpw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2efqwyjmi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wfntgnpa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uspxjugp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cmcozumi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eyrivfbr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mogpbfox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ckshfmey.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kupibyhk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2umogwjpb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jhhnqjns.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tsybhftc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fflaarcb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2isxggmhp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2srvighdq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hgoodezx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2uqiqubjo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tfznrmtf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aqxshgvf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rpgnyytv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2arrhncvy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zhehnfby.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwdexjjc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sepmcsve.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ighelbvd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kkdtrucm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2helhajhp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xuxjqmah.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2naglrgrh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tlkxkier.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opdcfluz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2whcfblbr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mgybmxzo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2itdetwyb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wtehfphs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2etezjdyb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjolblrq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2towebkzg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2uesnysil.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nglmnbgi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dtczhypk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bjhxekxo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kjujktlf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2khscqriv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lyuigrka.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eyfamyvz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hmjzmxsm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zulqbynf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qnnigitw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hywoyagh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2opsbcbsk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ucukerzc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mmmaptmr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nylduwcv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2leyqpcql.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjkuazwk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wbkssrsx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jztatcee.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2evkhlequ.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ywozzmpa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2boghapam.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vpidbsdm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tjcbfcyg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2auymbbnb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhxfrjwv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2samdjesy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2divqikiv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jmbxhyzn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2iqbvgkro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naanaskd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ulmbtxgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twalkxdl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rwtyuzro.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gzgtexwq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zitmmxlq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xgpkxrdy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xsqhliss.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywtirzmd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ppnaqcsa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ksmsmunq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zmsznxmw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mdjwibxf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2evicgeht.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pxustccg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2upozpvii.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2eumaittg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ssfeoruz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzefov.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hjhsjlpm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2poqgxjqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qcsqtkdi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2egyjwmhi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzvewl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sybdmtbg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2avvkolcn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ivxtglgn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xtavtjhc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2euabnlpy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ypsvgdql.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikwogihr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sahzqnsl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hzkvjfbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fcjmmulz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qainpkvu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2payuezgb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwmotlzd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2afghsvfy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xdczyeem.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqcskmcz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dhdckouz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lfuoykzt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vkgbnxqe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jiaxzztv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvrhgkhz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fymtngkf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nyzilhkf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffrbmwar.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzxmdopd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2neiyoyiu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pmpyvytb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bhnxtwwj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fizwftnc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2oidmboqy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgoboyig.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zluagkpi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fyhpnkhc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jylzilqg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zgoclmdn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2itqadapm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2emmadehg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mixasahx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jlouynix.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hvjisfjz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xefkrlva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tapecojj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ogdjbfee.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ywrdwmvm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfvnzyyy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmblildu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mdgrggwv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dbyoeqjj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2uqgrphpd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xsmcgzbw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jjyrnjvr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hoxvulhq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hjhdgtnn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2eftdlvju.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cpfafhgd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kecdlgqz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rhuoitws.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqszyxkc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ubgsrpal.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nnyoxamr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2slwavymf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2edxnbopt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvrvet.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2flpsmpud.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2njomdhmc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2krivmsig.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zbxisitk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evbiulky.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2frhgqxgh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sjindakr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rbtmmfpp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uspshggl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2girquebm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cqssyhdm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2filtsebs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dvcutocn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uociuupk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfnmirtg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yfroulfk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebjxrdfh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gqozrytk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vxkuslxa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tpojyfus.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gsamgkmu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xxspgldy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nwgicznf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gtcjmcuy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqqmllpg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lbownjwh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ukhxqixq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ineqxfos.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lxapdwcm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2sezaciqj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2htaqbayf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vlkzddqx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hqjtljor.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tfkepioy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bjangavz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kaggqhhy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fqesdadw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bcxzzzvg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bpbsferg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zuibhrit.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2shapslwa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fzowtlgi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zntvhbss.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mgigxsfa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2njxehxzh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2unydbsll.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ryqwsdwk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mqvfyurl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjvgsgr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tfzdpjda.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ukintxbu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nksdjrcf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2htxrmcey.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2rbjbtybv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ravbxtuh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kyskljsr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2utzapjnc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2srkgvcaz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mfszzibf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xqqhbsgi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ngaretla.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oprdxxbj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kxggvhrq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qqsximgj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2skvomjyd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cpvwhcld.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bmbdnspw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xhnovpss.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zbfatslw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lxphmgtn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bgmpepgc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlcsyotl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fbqszczq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2icfbklhv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ejkvhmxe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dvvuqgoh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vznxpiak.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bgrgvfcf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwmfswdv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ckyvsipm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sbwmytwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzqlucdo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tpknssnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqgcmzfg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ijibjmos.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vkravitd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjeettbw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lnxhtrme.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aqlgohlp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fhtnbmvo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2deginhpm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hxwxlhtv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ygfaumau.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ehlcbkdd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kpybszpf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2czbdsiiz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnligh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2epjanpkh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pxyjayge.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qsrhzlbc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2crpuxuad.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qloujasp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yuynbanv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdqkwp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ojtaxvwr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjepmwso.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vzkibyrq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ztoepfis.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lucednbl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uniopxsu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xjrecsoe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hbollyow.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lhagpxzr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sufqgohd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cvrmiviq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jbunboag.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qeciyhgy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bodllhqh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ekasnjvi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ucnvhdfq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2degvlidq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fapsuvcy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sramlayl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nokxbpqc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gvevqfnm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bpfayskp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xcksxecr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2culzpxti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xsxtdpdf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2azjtesjt.html


<!-- 参考信息 -->