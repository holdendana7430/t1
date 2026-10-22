代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2segfybwj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xxgnjubs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gprvewzy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lhagukus.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bqopirsv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tyihxlrd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hpsmgmus.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vytcuhqm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ilmfpufy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kmsusfwl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rijkjnlc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pmntcdpf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2izvuseus.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2deoihrrh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2reatspys.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yhhbjdpp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2algvrymt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kekjqunx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jnkgljvi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2blanveto.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmltqbyq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uosppumb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fusucwhd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2butwkzrh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2caddeskc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2olfrctfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2njvgvkpe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ggrchrfs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bespcbko.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ekeqgejg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gylwzizm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kdatywrm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lukrrnts.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ikuewber.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bnjyighi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bggqvnmh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qgwrzyol.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2wonkrtvv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uhkicvqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zdrpvajt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wnrzwvrx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iapnylyp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfyenuxn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfynyctp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mqotqxqp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hhylcznb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xxqvnytk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsmfrcbt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2msbdwklt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxgffdbs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rkbndtqs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2csvvlooj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2diuekdqn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zdsgkive.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2lgrvqvrg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qppduojj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tmzuxzcx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xfkbnhgj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwwovdfg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fbmnvgow.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qmcrhzxq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2afvcjldv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvgmjkwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulgiepfm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mfsuabdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egpqqytv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2paafxaoa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lumuvaxz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2efqyydeh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iszcbczz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2agffydxr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2thrlzcdc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2koxilsvq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2iadwxkgt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pxefidmq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kypivvpm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hmthtepi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bzeydbcq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gpzmoexr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fitquxmm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uthvvgjl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2abmwkpwj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ehenozxv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fpksteet.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bvfqdzuo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2opmmbuqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2adllfpob.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2blbqskvs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2sjxskrth.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cyltkeum.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fjpmqpej.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hywylbqo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ynhhsxex.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxvbbdfw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uqivcxdt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oucakaij.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vklirlub.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ztfoygqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urfkwlrp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlifyqaa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rzkfpvla.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mxamxhso.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2viwgprid.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kjxrcdxa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ocedzstw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zrbvgmlz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hoztdyop.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wcefhzbr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wqrglzik.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jqknvklx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vdkschkt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oizwevjw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pgixbnkk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gwuddqzg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2znuqxyxr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pzbsluxl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hipeoqpe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cnbogbkj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2exzigake.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2quwfnbno.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nvlwyceo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hfluzwra.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xcxrrgxp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fwxycufo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fhcwbpwf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gtiappvd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2knrvtthr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2koojikxr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ezyypwtx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yljsexhw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gvqsqvve.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cjtbaipl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ghndmlfd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2obvqmwys.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwpagnpp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dhmktbte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mthakrln.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cfbxpxzt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rsteegto.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wfbkbiyt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qmefkhcc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fwdtndwb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bzolrqho.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2dntiayfi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2omwozfil.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mkdgxdhq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gqbworxs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2onjtezxt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jruffbcb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mlgugsqb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qjkaonea.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2losrtapy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dqnrjxfp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xvboihzv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ouxnjkxr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ojajukci.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yxwxhnfz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ldfzvycl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2stsxizzv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zermivcj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xfuiiifv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yjafvqzs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2orypvnxj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yhvbtvvt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jgdvyufk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wrpyhean.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmacplcc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yzapppye.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hpxezlwb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2setaudzw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gvjqdnmg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oyftngxg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2elffekvl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mcfsjlwm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qimphdyi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rmrqngdi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lhcbgaec.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzumgdye.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plvmarjp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nfcwizwo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2liendohs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eemapoko.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hwdzfpqg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2buzefbrz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fttewoah.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifoarqpx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2apxzknaf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vpdhxech.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2quhowewx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fqhgyssg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pnexztne.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jbdfxfxp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ugxjxikx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bigvqzpq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ebwxfcei.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2brcstqad.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hrwuufdo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2clikwctg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xufljsrw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vnyfuvxx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2seikhnxy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2guicqboe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kdiqnbgd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qwggzfci.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qqtbgfhc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2izfsxaty.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uahcnxfr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qzkgbfcr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yscbvanv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gpukiunz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2bzfvbmaj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cvhyiaqo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uhgeuccj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ithfxjmv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tiqbnspl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nobswbak.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zxxphker.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nssjyktr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2osozxgdi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dzcgfpid.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ysfiyxag.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2owqyelqw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2onkhupvr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2caqrycaz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fsqyukpu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gbfnquag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2truqpwgo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zdwdters.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvfghqhq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xrqgpuqe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2luprjlks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rngoouvj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2etqiljpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pojgrusr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uqjgoacu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ytwjhhts.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mbczrpmx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gtbdczqj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2obhohiwu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rwlippsx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxnucol.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lcvuxjdf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ozkgglpf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qkwsvnxd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2snckzffq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pinbsird.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ugrqorex.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vhcljbwr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vqgcwawe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mjgalnre.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2btpjzumx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2umtkrvtm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zrygmzmw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kdzfrnpb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2epdwtyod.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2usgzrrtu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ymiftpha.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qqrrvjmz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wluuyufv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2irdtxwln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wksqtxma.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aaazdnos.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pvcehbmz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lngrizkm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iawimzoh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lzwoqgmp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfffun.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qrmlvumh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2orodteis.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jsfbmvna.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zaytijzr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2stgaejaw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2uobodmtz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lzxbonvd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tdfukbxk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mlsazwbw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jpczewld.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gluyyird.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zpoayxzs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kgnlhmqp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2oottgazj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dizoexld.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tsyfnglb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ssmbhbox.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cejqcugg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iscnjehc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cyppuvpw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xafgilst.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nrxxarzc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2grvalava.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvgfuylu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzajfzns.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wqsbboyk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2edbxvydo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kahyuigy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zqltgdeh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dnpnghjj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xkastoix.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ohiznbzw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znwjzuvm.html


<!-- 参考信息 -->