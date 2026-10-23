代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fifcyrry.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uhhkqngy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nmcbksnh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jiiyvyhz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcrtguwr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pueyzgud.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iqsgyenb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hofxcufx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3znzlaflv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wdqismhj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3obhlcbfp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rajkbshe.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mlprqcom.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xybgyebn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hmjokxxh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ayrynheq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3veeewdix.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dhnlipai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cdkowsmi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qccsqmhc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vnjoucpd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pzsygvlp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3clakhfiy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kpyuyfrb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mdfgxpsk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3incsikug.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ziehncai.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3thrvbmjk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pompucpi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gghwhjzf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mwraxfdf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcwansxv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3optejytz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3elkeavss.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ezgonevc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbawylyh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3czthzpvt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpdvwirs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rczwlcci.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mykjtpxn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3stoftwdq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vmbuuudc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fttlnipr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qeqrsbgn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nviciphp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3citiazlo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgegwnkp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ekwzeawk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gqogjpem.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tvsiglwu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cbzkjnri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcfaqdbr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jpvnezzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwzswiee.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lkaynevh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fkromzig.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kihrdfcn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hemrxueb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xuhfgpvo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hewhwcgy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yatvrutb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3migipqbq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tvsaoris.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xtjrtjeb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nyvaivfn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3atxfbqtr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeudpcha.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3aeamjjba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ifujopje.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rfwadmbb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nvmttnyv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wjojuumf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dqocqneo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qqnnzfok.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zodkoarx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3syodnsgi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3rhdwnnlq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3owypjkth.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3injjmzaj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xqkavoqq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3suladcwx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hiqlowhs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eoaqesfp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vicnlsfc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hwmgazme.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3elhgbfur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bmaocvqk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcubjsgg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uhhrsoub.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3epsunwsr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhdonley.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zkarocqm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jqswbdzf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3sxaphrew.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ngzkmvvj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lullqocx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jgcnvhvm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bvrnhcdt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rlgzznsl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ddaaqpxq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jfyjagqe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mmjgaikf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fcwlegyp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgtypndt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ylztfvud.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bsuqiltu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztgkcgpj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xjdftzqb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vgtvgcgk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3scdwyjhc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dytujfly.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fyhajwux.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xikoamqo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lhdvddlm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xdgunrqo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3luwsfbof.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mcymvpze.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ddxqrpuy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rcryczkc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cglvnfup.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjikcvr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ojigqkmn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcdsrmhy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rjeedcxk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qkcgbhmj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ohsdzdmp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jwzjezsi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cadyibok.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mqvtjisw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3idxivrqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ejbevgjl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgqtagld.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tylsybxw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ojnalbbl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tllvutdh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qjgtlmjj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rjpyulln.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cffavvha.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yjnraexy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fqinbogn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sfbudjez.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pzhdzpmc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dliybsol.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzvpugfc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mnetruro.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qwdlzxbj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3eadwuqlr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aqiwwxvi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qqdwqfkz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3apxyqbuo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cvjgawrz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hltmxphk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xgmirknm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cvzmwreb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ocevjnec.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lzrhifed.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3abtoqkak.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qflprwgr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eiitqsbj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fdrnmpwa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yeltevkg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ibamcjhc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qwilhhir.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ycucraup.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3snyulgvi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jradvhes.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vpihpmpl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mfmbbegb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ubfvikbq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jeqcxadb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ljdfugkm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vnljnaus.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3odzfpwnp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3cvcxubzp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rukeaqaj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gbgksrzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vhdyzrpa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mkesjniq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tsvfzaez.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qaovthym.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kpvslbyf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qcnzgvrd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nrpngxmc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xcflcddw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3radoudbf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tcibpcsy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3frozvyqa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bikwycmv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pdliwgzu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odzpjehv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3agenaeeb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sgufgpix.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zacnocvm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bpcqdsmi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcvounzl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3onaunzaw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3benwtaow.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3plfijqny.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cxoqvbvv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zyedfhhy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3czgdxiws.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3whbemcre.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gtxfcehy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lihpqwuw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yjgeegyl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xxyzbbcx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jrhffxwx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oddjixwn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wcynkqhy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wiauyrmj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wrlggilq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hdeupjuu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vetsxdvy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3cxiixezb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3radlziqq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oefheios.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pjolyjwx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dbjhiwwb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3umeyqxgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iipczmux.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wkrdxoay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijxkansh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cyqhpauk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fyhmyqkw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3czrgiaxh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xociyqvq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bpufnjpi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3piodfsry.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dlskrubl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3palyyjtg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rfcoghsq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uuiktmbr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmwjsaq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zvctrjvb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ryedfoyu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3roarmiye.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uywvxoec.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rpzebwmw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kijnxktn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bawchmrb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dngfuzrc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lyzvtwcd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xufwshof.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqmhrdsb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qqheipgq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xnuqrcwa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tlgxrnha.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dxwkxwhr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qkfivyrx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xpdydgsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3sgdaxgnb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hwnpmzbj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tpdtttfx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3beyvztbw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ggsjvmiu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wpuprlhz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sfgomtqr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njlrcadr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ijuhiozr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kqweixyo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ykssrdjf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aptnzjde.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nqaxwclr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tpitfmpa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wdtalajy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jtoahfzk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lumnssyn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xnsjveak.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ovvxwnat.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yiygcejn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ojqjzvfg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zxnfyqha.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3btbugijw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jlcskuxn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ulajutud.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nyiihhui.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qqcyrjpg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3whphhkal.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3moexppuf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uteajnqj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ubsyvtbx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctrwnrbr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bebopbmx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3srjqzxlm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3oernbklu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gitgnzso.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xzhskjee.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cieifyyz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ngwbeqoz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mduzmeco.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrhnfhch.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3awjbbxsf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fyrxsrqy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3grcbxdsf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qknxjiah.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xpcazvon.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uevzwnag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnfakrxz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cynpwvmn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vzruomxv.html


<!-- 参考信息 -->