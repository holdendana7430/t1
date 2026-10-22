代发 wailian999

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qjqohwer.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zfttrzvz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hgmqupzs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2akkaoqxv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2flspxjlo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2srizrazg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2frupznti.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jbyjbbdt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ugypbkks.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hnpxqces.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mejxppjj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wokjdrtf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vzvuscqp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dvbbpcfz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qlwljtdx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2taunjekl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qfkvlapl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hrfmsdvo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qqjdasch.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sgeqzxoh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jikcgkav.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jmvsemzp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ltkfoeoo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cjcjpams.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ecqgufih.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vfxstgks.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkizforv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dyrtgxfj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2imibwpjs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ovwdauhg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2odenqycm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dacdzzat.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2feeejets.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hzrhhsbw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pnhyyctf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kqteoehm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2aiuqymkv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urujbash.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkrosrkg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swcxusib.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vakflbim.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsqsopug.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vqrjerle.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udqfsbkh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2minptraj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrccwcfj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2actdeixa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2udtkcltf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zhhbahku.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xiglnwfe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2atuxkhgp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pfzrpzgx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hucppwyn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vwrbdjhu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfrnense.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mlubrnlz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2smcnvfys.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2szfnhxiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2plmbwjof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cisrbodg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lgrhzvkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmkmdqlf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lxnabyyq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oycsubpy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ucrkntuw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gzvjmtdu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yysqwksc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qizwomzw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uwtroebh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vlfjjthb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tikvkgvm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vcsvgfoh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nfqhcejh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oautfrjt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ozdjsiqj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pgotiqqo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hbnxbsfg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jsdnwsur.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rcvxbkvh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wmcdfcxt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mvbnforw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dmwzycsk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cjlmvynv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sqrbeuoj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rmizywvh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxfdkg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jgriwjzf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2edocglml.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jksolksa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dmojltsp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjfcqhsj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2plgkkgns.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2exxyiigd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ccdbggrf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gpgkfrkq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2myfmhype.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oovnizvq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2brxssjod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yixwuoxy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oylpecpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2itivfcpe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2adfvauhg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2awokobkc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tssrsnsv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybpcvzuk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dmkcahul.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbfafwdz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ciwdbnlq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vwrxhokq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tuyszcfz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2boprfror.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2brbygbfz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tbxsdqoh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zpskthci.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahguemco.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fttkwtdn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cghgcpdf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtibkqmk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pcutwcam.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2itbqrvkx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2phvmjrmn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lnnibayn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ixwdaden.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwknjuhv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nbykpnhy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nyyfebbw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lithkmmo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtbpatgd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pdoypxeb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2klarqvjh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewqpwshp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kinrsbjy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lzavqmbu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2estfayqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2aueiyabu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2acuwvmme.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ymbfisoz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wbjzwbui.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ysfccevo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gzleqsxb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwxgndcu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vslmehcc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rpkgwiyv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2umvrqivb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wiyqopfk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cvkyxqlo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2usjkdpoo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bjylbgar.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zcmampct.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vhndvrkt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfypmjcl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2djpuuuuc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wzooqrcd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kjqwcksa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dhedqzji.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zazgnwkf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2umyypeke.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2uzcurrpz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dqmdbvxo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ymmahqke.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lbjttuav.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2azrgrhht.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovesrnug.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nrhknzrl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ffiojbxr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vletxkwz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jamlfrle.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bmxjgpdy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ocpxpofi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wvcwwcwo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nznhyxjp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fqrfuqgr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2cjklsdap.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rewvzixy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gzyeskhb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2pqpqchpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bqntxssh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2slogtztk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qbrxbejf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bxnohsrp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nhiosrtp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2cuqkxthz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ebkolobp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2owlgqfna.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pasyvqlt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ufobrmba.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gdnutyic.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2akdzekcc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vzxxvpla.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwbkhlhq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fgsthvaf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2decsylop.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xirmrrml.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2izsxkzkd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sczcdxyv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ajcdxqar.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rxiwxaan.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2anzkdtdq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2snvoggge.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2phbiszgq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hbyqvavm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lptjaxcy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlzmxjsd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fyqywevw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nevwnezi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mmpttqkj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sdqmjxex.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nbwldmdq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yooibsef.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bbzopisy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcxaxdwa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ikwlnjek.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bxhwovdx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wcgxhljz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mpzlgvyh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2suqkcoyd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bcyisfsc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dfxamqzx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nugqxrtp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cnbaivgm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rnrubdnb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rqtzlrit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tksxmpvw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bonisiez.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pchhbofk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2asncohvf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dzqvlpmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgczjugy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2atzfdksl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2griqeqjr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggcrxpqr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2itoxihch.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfywghry.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mxfdlqab.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bvohhmhg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2iecvmzvz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2booqcrzm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jytiyzxa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pzmykpmn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ekqdzxbb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmfknbq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vutdmqdh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2epdwtosu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xvdgdqce.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xsvmwipi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hgfwstnn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sfaumeuz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mgvghrjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bhyqdsbg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ktjtbhma.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rupuceed.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ojmfbzfh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qxvyiwqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fdslpiyh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hzmwunfy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yccnrood.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2csuhslyd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gghioeai.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2szeqbpik.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kaseazul.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ccwliywd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ppwkuxhb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xfsnrqjh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pdzhmknd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijrfsodo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oqdllule.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2plsevjzi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijpiuqtw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2owvwxcki.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2axkcvqiq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zyvryuea.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ujuzprwk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iguwhuzt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bnrpcrfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kvxmbopf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wvlezmhn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2blhmrvau.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xvyddzjr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2soqeabjx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fgqzghdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2paufmpao.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ncuiquvz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ilpqqpms.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xhbnrwxo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wcysdwci.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uchvueqj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ttfbdeyh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2voousjnk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aptupvck.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tprtntmw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dtfqqmgp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qvekumfx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wwrwapgi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ltnnpzie.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gdsxvuuk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mbhuicob.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kvynemee.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vjfhyqhz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rqdwbmzt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2oyfeqacq.html


<!-- 参考信息 -->