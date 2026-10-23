代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xkiuqehu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xnbgxjlk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vbdyhnyb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hoaidqlb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mqogwhuv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iowjbolg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rtciyqca.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zjmoinmx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rerzcesw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bimgekvb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtftlblh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ttwakett.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kwttuezj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qakqipke.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qdtarybf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dvfdqbps.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ahhteggs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lurdsbda.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wivjkwdm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3akycznjf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3beaszcgk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ridjuzjf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3svgborws.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fpnfqxyf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3eohjaklp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ahmggarb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3plibgnuu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qviqsxof.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3essivlyq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tdufaqex.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fhawylvn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pwaybdye.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3phvuwvwi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cwgvhavd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kfxlshko.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3oqswtzgt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kuwrdgho.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gpbbantv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lbpdffal.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3uqnlabks.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xlsspvly.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3tgvhpkhc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cfdjqcbu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ooyarcjr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3asdjubam.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qzqrtjtt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ncsugyvk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3drtijbfu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lujiuyyr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iyswbnld.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nzwgfcvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zydhvuby.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vorxdvdf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3oqppulzs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nyhvegfu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lokrgutn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lxqhmtxs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbmknbua.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gwoogkti.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfasnioy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3apwqqdyy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3syuopevs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfaihqqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvabfkpi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lhnegmmj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngwtydxc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fkszxnac.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jcbkwzgq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qikvuaxs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zsytvatg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3iwrtpydo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hapurxfy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dmqxvfww.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrogkp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nsotibyr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wyrnbmhm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qqnstlex.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oukqxbhw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dvjwjbka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyypinwa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wgjtqkmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yarmqnid.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xdqqhrza.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vhrxsdoq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdjzzl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lqahnfbx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bhumooms.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kdycsslm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ccsqtjtw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lmhvczcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tpatoqzd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gwkthjus.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rokcwalo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfcqpx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3atfnlssf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3szqiyklq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sxipbruv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcogebol.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kixnopmu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ggzqtada.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqlujdnk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3adebqees.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rtvhoqwe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3odydusuv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3brjndflg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iqprldzr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hnhpakox.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3elzsulkw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zotxxuyy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gsazeaap.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fviomxlk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xerhczsz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wncbswqc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3brgbqcwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hddwcmca.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yvryxkzu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmmgdfvl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kdeirrzu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnnvfply.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cszcfcmy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xybaxamz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3utlopxmi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rtjakvzp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tzidvwpk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3egpasugs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ngvzzuto.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3flkzywbn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wfqnbtvs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bsdasmbz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3snfalnqu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qxfpnfat.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yzqnwwtz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3twrakykl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zqsnomsr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gzskebdz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bipobzbk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jyxqpvjf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxfhisxx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wdhycunh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tmgfiglj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3enjopimj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3octxsfwb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lxwoqkjm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3liuipsmv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3owlcyigm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uiffjemx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mwcyjxox.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rzcqwtrz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qxzltucw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hpnkyvxu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtssdfsv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3puiwwiji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hhwwdvfg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fflkjluq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rnkjlsac.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cqowoodh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3alfubeck.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dgguwrlh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kgjfoytu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajmcpudo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhobmtib.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rrkelvjs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ozwhbtmh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dzguxdtk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sybzijfi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3apmsugsp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3taranqrj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjwughfp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iatctokl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jnzxsupt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3odhtducp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3odygooqd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nvdiamlb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sqsiaxze.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3iujegjca.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3agrclkfe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vhryepex.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mmtwfpvt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dmxosenm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mombjynb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fwrgjzpc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oafeaxmd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jfoomnqa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3niqpnpwq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mltgguez.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pskzghbf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eeudvlxu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uinddezc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rngsltik.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tmcdzhgy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3chdonxlo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vwunmbap.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dsmssqcr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dszblsdn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rchliihb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dbumeylw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ebzgvnrq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ddhalpow.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3klngkazv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3btaryfbb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uqfddoqx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3umztmlth.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pdrvicuy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3krowgidk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nhvfdilx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ztpnjdeo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rahiaqru.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bufewkel.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3crfhbidg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bmnulzvo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vvhublai.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dxlaxkom.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3elvygfgq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yarlufdp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ubggqpxu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3szszgrkv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vlnhghkl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3agqiadtb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wjmbitdw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xnlvjnsq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3eagqdcxl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3kdizumlf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3byaksxyt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3llqkdboz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fohfcsbf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ofhhvxkh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3naqyhqge.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ceagrqlj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3khejtnix.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqtwjs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ixhvudch.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mtcotrmq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3eitqppjk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kmljlfqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3opqqehme.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dvfylybf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bpmmiewd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mbspytpf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jbbtkavt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3chhgdhpk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tipxlxtf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hscjbrky.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjxoxuuf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3relpqyvc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ranaewfh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vgmjrvml.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fusmrrfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfxqbzae.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dmtwylcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjvtbiqq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3anbrukvi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sfmsxezf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxunlxem.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gdulzhlh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bbiamppl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cnylydcg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mzxvhzbj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mlszvkbh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3estnkmnf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qyxpllor.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wxoldoym.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wipvbuxs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ojanvvuf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vqhsavga.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dmklqptk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jzkdhcoj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xdktdfds.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eanwrvpk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3flprylux.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yftdkzyn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jkshqscn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3akxkmthi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ykgebarr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nfigyzqe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wdbeeegg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqdwxast.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3eqfsqgao.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3aszqfybi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zxvbtces.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pocgoctn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cnquzkhg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3epdqvtdr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3iqzrgcoz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dzgnivdm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mozilhnp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ggejhsjn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ufdcsvxm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ktqxrqjm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ieiymecd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qxgbspzv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cgjdvpen.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yswkrljp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjxqfw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3drfbdgjx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3awxadxlr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uvkxvzzl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ntqmeors.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3urewmskv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lhmbywab.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ilmejrlk.html


<!-- 参考信息 -->