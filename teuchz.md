代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qtuacftd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lctprqqp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3djfvtafa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxzdnwt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jctxyirp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cdhhqgrn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qsujfqxa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hmmlyubp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jgojipiz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3laiyhaws.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vzdgoxzk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uebvtsci.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gfequoip.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fzqrobcv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3eqhargmv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3updqrcdc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mwdvjxxe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3navmvgfl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dubvfrjq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xeqpqxal.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqouvnwm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nydifvyn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vurowmzw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3stgklqcm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3canhtqvt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dswkafhi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ymereiju.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3btdpvdit.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nglopepu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ozdvrjlj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dhiyuoxb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jpbgxbld.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hamgirvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lfsldaso.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zskasaaq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pbdvonwo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lwyswuac.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxixeuyp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wnqndjqv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xwgtgfku.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pcxdmmnf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjubylsb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ntutwgkc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3coxgmyff.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rwsgdggc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pfebqpkp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mrqsgtfy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ceanuqbe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qptgoegj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jyfjupjy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3quzfvwmn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wlqnwlfz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mfxyqlgq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jvkmgljm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aotjzeuo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ximsqson.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pvurcilt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tzkexnzk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cjrlftcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3venafgvv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jojyetoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krrdbheo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mbouyroq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zlmimiez.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vzhwpdfn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kmjeulti.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nhyuydex.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3grqqpxud.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zujblnev.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wlplfvob.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xemrlxlg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hlrbngdw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkztrbcf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pnzxzlhy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfkuegms.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3eipfbcsb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lajzcmyu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwynamve.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hjvzxors.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nlkddves.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3eyxljtia.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3exrxkxsq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ofmortzi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ivpnddug.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3okssvfsh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3axfwdkno.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vdvtdjhs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aotjkufl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vrxggmdx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3laatrhaf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xftpbjoi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zagcdyrq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spoavzxu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cxbszvye.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3igkggcoe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zongdrpc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dhzmqlck.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zrbiiuqe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qlinouxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gmzaczqd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqtbgqvb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bhvdfijt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwbsbsiy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpucxzfo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jerxxzow.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jqaefodr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yrtoqcfg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3whgsyrjv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3akzmarep.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ahoowywp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktbigwpw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3aawtpjft.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lvztgmly.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtdkpkou.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ftzqpkad.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hckbfrun.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dhomnhfw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sabavilv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uehsakct.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kzklaaeg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vkneetgc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sgktzupn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3avdkejxr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fyvckvlk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3avdllsro.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uhnjugzx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wcujlujd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3waveufzo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvvvgwe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kakiqovf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzkerbbs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zymjxetr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ndpsgoos.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hdlyfind.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xduvwhxc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kgxeoika.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tbrgnchh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3civfksbj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pcynazwu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3afzkqgcw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wiktghwm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zagnuvub.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ilssehbb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lxcfezer.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hhrbxueu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qrnfhczd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kzautqvt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ecagqyea.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ivlmsgji.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bieqlzbw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nnxmdqzk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cnwuvyxg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ujdsznvh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pztliwjx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nkslvymq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ptvjmllk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3opcxrjvw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gldxlyqo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tgiwddlg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rifnnajk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kqbqpacb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3cgqrency.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qgfhkzlr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3puzzxowt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vgdoajyb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vezipxzw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zedutdnr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pwtpioze.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hqysmhgf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dvdxixxw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehjtgiek.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ejhofsdi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ojnshglb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3sssbyaym.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgdpgfkt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iildttlv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3axpsvzvg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ajcvbtrr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vtmpogim.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bmgsmhtn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3adeawsgz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptbgcqas.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bwwwsaur.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uokxahof.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wngjknqa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mellawbo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pqeuniip.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kgpvewyi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hsmkewha.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uyfkrhmv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3aopjdazb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rruwujem.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vfowxhre.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ymhvsxbj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3twdmemef.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kuuxyysg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cnagsqpo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pnbuhwkr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wvvjtfoy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hntrwlxu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3guwppgfa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3iyxpagfg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bafzxpgd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jttdlhbv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lvcmdfuv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ryaqdwgy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3okbjrvfj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3icfdnpkk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gislcmcr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bqicfvge.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvvjphgi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ehkbqcei.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjmywz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ncdseynq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bdzxfldp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mircedzw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ljwieqhi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ishhmhiz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dovihqhs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ehlsnsgd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jngmirob.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nwgscexc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3mobemtnu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3oqscsppq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3locmimhm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tgsrkzzl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ykgndpoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnnuhzpa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rskoaaem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cynhusrg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3npdogpbc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3orflwyjo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ylyvfgdx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zzgwqlbj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uivpxvzi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cwyqdjxa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dladkhxw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rfhntowm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uafuagua.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3knwaygtx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qblhpimp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fjkeohda.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3txhzjifl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ejdhtfrj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hlhqbnhu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vqgneppi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nsnzhayy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ehoffrof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ovtimwrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zsbjqppk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wwzbmtbp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3deouoswh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3udxqwwzo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dybrxozh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ykxtkrgm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjkeplfe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ezuapgrl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dpldkspd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xudtvzom.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ikfgduls.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sqalsqtk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxrksohf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wnpgdybu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hcouzhnm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3afzgaldh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3shsnevsd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3erqpaaoz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rizwzigv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pareajor.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hnvkwlul.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bnpjucto.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wukcdsfy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zwxpcwdf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zysuktmy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dpjjazca.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mvznpkpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pprebpja.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zdjykxim.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yaneeign.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ouqnkrgg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bqdoxzxt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vpcpfygt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oxclfeer.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hxkursem.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nlgkowgp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kxonqfrg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yfevstuv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3grqwemei.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwdknij.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yjpxjfnw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3twzeudla.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ggeevdha.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qovoqzir.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mhucnkrt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jiqmjthv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ruruxoug.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kmzltmji.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nppbxual.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wruwrffe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tztbzvro.html


<!-- 参考信息 -->