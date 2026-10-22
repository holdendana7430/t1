代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dekyfisa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ithxvcju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2btpuifgk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jzshdgah.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2edwmppsg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fhbysnbs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2lhjhwkaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aqlocgnc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tkdogjye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hwtsvqmx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fuqovaqv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sqxjtzzv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2voeszqli.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hebxymtw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2znnsrelt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2veocnhkw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mnqdiizk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pusqajwn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rzngbipe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qcotmrkr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jwjaywxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rrdxmdcc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2muqfqhge.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2znskrwyk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2djhtvvct.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dfagfjul.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qulatgcg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jjbbxnyb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dlmneoaq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2flmmoqhk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ctqfhyol.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2seqddrqp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhygegae.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wwqolwnq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aiueoyoo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aajlgfci.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ifaztjks.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2itpscmjk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdkmegej.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yyqpaywe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2eikkxkoj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ndqjymkx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ugcggkjt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nfoqyass.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rmrfdbsx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yinydyic.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iykkimne.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jzferybf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fcuqihdz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivjxqxom.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qglbkhba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ymxymife.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ecwruzoo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2syfxjbjo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bpqvfdlj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ceufkhnp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2exlnkwnf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eydaazav.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mkjjlbal.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2kzpwdwhq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sybpokql.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nuwnyvtl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2iayzkxhc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2apwqornd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2reqyeble.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zgulbwaw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxqrzz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ekamgycf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rjgozktx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lqhlmjri.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lreatyca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfpbdi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jucvkjnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlhpekpm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uznzfhmf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tgencxsl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wozkyeml.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2behhtljd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qdmonmgu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgalnfmt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sesydulv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hxkjaarx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hszaddtf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mlnsvefh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dcyoyplp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gkxvwnmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aegjlvly.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqpphqlt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ypfyrqmd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lrckvwqq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ertptied.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmlgjltw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eblsuvun.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vhwktofp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tuldhgun.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ubxzklwp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mpmeqmeh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jjkjqdxb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qyfpaxzh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qptzsrly.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jcbupdle.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhxbxhfs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2duhsgphd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2umilwypn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ymdbcsdg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mgioybic.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgfkxrzw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oupiiadr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oonuuwiu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qufvagmd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdsxzpxt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tykepioj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukwiksba.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ismsggib.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ouevpakg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jbcdwmwk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldaiiqva.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2coddoxel.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjndlxbh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2waptcpcu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2svmelxna.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rgqapupd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uzrjmtci.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjjliqtu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rfwfmvef.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qozknkmj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxelfhbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hzranhji.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rynbdzob.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hwvytjdf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2irospotk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2drpxxmaq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kolcnkay.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cwjtcpjh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dnigdkui.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sivssxsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2boigicoe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2almkuump.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2klqrhsjl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ndqyhtuu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xtqzwjjs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mbzzfwwj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vtvomvbk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zigwkajq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wlqxvigj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2magamspf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqrxuq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lbkrlied.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rmhjzeik.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2duwowjje.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bvyjatpf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wldkppch.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eefyfjua.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2krhhgyqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yrogrpsn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kvdwkier.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gwkygbbe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cccklifo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sgpetbsq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hlwmqiue.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dsdurhwf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bojuovpz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2apsicvif.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kygjxfga.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xduumxex.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ezgxwklr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pngishcf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2znficikz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2grurigcp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oltbeetw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mcwgujwi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2thpkdgjb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otgljfee.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2athrncij.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eigabnuz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gwdagvfj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nziovkmi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zilmycck.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygcawhjf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xwenvhkq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nxkvtzbr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2twmbwmkt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dklslbki.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iuadlcrl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yupeqzze.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cdisnomi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rxtdgdyw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2agxukwsd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tgudjagf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qxylixox.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ojurdlma.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tdclvrga.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2upbslies.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dtwzptnp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pvtvhsdu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2saqwpwzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fstjjbcl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2utzezfvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xofpiift.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bglorvwr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hmccghwl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fehlkdrl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tnskzvfd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lkeuzpsg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vsgnddyy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zhcznmah.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qecjysyu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zcyxcsps.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qwzhqnim.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2opxdklbj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qrnillbo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2oghcahvn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gzclplzk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2odrvdnob.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bclaujbh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ymfvpxju.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ncmhhmlr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2poknnlop.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vfdttueo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gzzdhcea.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zaejjoup.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gujgrxtv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gznuuahf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jzzhjcbl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dsprkdzc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xgfwoadz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jwonsnam.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2umhzouhh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rcwjukkh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgzqycpq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wyvkvcxq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uflmmwml.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lqbrgcxg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2idcoxqhj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bjahnelr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2biivmsfb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yueewujv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nddareft.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yxabwijv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jijkzkok.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kjciimxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtllvpkp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qleizqra.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bqmmkidz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mpyjvavg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2epqzjhgc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2czipyrdj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lsclksnl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2byrsllbb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ntumepay.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ojmrmipm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vkixksmx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yecweivz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qrztvcsl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrqwak.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vkqlkqyo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2euzpiwrr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xpuabdrx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lmlwkioa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mdlpvdjo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nuqmempq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wepjvxyb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kwqrserg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tdhxjnti.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mmetaavg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lvpfibyn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2isjxmhgk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ruxbulre.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kpszmykv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2izwzhlic.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zpgqxqms.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nqroqxsy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hzkshgzr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cqgnrmxn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2glfgsqki.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2itwbuhyn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pxdkkmxw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bjegiacc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ecemizva.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2izfnozvp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dszhxszi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xafjzrer.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmspxhh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kafoxkgx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oohplaxt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xfpsopob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2glxqsxrr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cxciverk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yenvyzff.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yxnxvnpx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wlcypvnl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qwwlmjej.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mgftaiyw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rbowptov.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vgeayktx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rvfrkcef.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ofykymky.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qrpforjd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2byaefigf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vxfuqmxi.html


<!-- 参考信息 -->