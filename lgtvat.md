代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pgglslkx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3eslfyqge.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bolqpute.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uendwoax.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cbgygdpq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kazerazw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3syvyxwtr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3crqokgny.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pvgqhweu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cxydwbka.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3emdabpvd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hsgehvvm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vyozssdw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bnbvwalw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qjrqvjyr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ejsmqusj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qnbrgimq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bvgcjsjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jywvqdhq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mhfphglm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvaolpbs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3muqmfbrx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mnyynytq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3evmvfiry.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pzoawvmg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bdvsdczb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qvncylkq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3effvqdoa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wynykidg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fgwjiari.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3onaebehx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3swgkbssc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bkxnokyh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3katedspw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jdlylulw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hwavkxxa.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3orbsurxj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cykbhwcl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rjssydtk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jajdmmey.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xbctnqzg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnsfgfid.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wtproljq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzelxupq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ribbgpco.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3femsmzfz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hrtywped.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fehtntuf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3abjjcejh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3szxyivsi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dhnxcwvj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uifdhxdp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gipdqcdk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3roejeewc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvzgngp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3asxqmfjk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zpnadzeo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yaerfhkh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ygqruuwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnxcvtkp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qkrcozmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncinazkd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3avwikglv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnjerz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iknwdpny.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ojmvzmcf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fohmyoxz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zewbxgkb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uyeavgvb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3slaazevw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ueeprkbb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iqwrceft.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3deiiedck.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wbnjbtoi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxbotby.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uraopdff.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fqwgatwy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3erhaskzg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3grgztyjv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3idpkgebs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qfotwtya.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yyzxgewo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dbyvyxwc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ipaqoozb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3biwunttb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3evfcalpd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ixdoafuh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qwtgumtl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dpehlsgu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvjwehcy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3iyjgueje.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vjdbwboj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gluhcnhm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jlipnlrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3twepmmvw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtkukqep.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uztctvcv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rsguvgln.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oopqtlvp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fthymadt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wqglevfo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fjmebhoq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gblnwjlq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3upeftrwy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbadvilq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3tdvlygbi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wxohvkjm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwzpbefo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uvqhuged.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3naojvydp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pnqvzryf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3auraqktx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dycqkfli.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bghowsfo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bdhhhprh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bpsfufon.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dgxizsmw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3obeafggt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mgqcxsdm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ovfutcyk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nbqdvtfn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nmjibosg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3evjmyraw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3behrqrnr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3eviqlodm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fwmvkqtj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ukrvsrlg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3idpxjimu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lajhilfz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rumdyidx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xxgwmpix.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3sdtfmfrc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zzkhwwoc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3sjervwpv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3inftmmus.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yumvkewr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ksmxzcjl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tnvsxums.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fseilira.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rkqgkoam.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yfbqbljz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3orxueprj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3idqoczrg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xtmnzrhr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xsmtpgbr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rcgbcgxi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hmuaejop.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pxkktxfa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yjmfadoh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vfnrjrjt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwyptrzt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ofrlfgke.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tcrhtacl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ukcqkmxe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ylobimor.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zuezrctt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cpfvtlsl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nsnwsysi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wygrdkng.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ytvlrsdk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jsmwwlqp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zrfhselq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjsdgrcg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3poxxhcyl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jawytxqo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wrfmvjwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zbwtyjqe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ljlwigts.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3owdzziiz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3diegvild.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bbznjxnf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ovgcpjjn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hjmoppyu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xsrrrbua.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbwnvmve.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kgfghaun.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cadsqibn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3etgnbedc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cmawfael.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xivloykj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3skyhfvwk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rihgvwap.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wzxvclbk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lfddnpqe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mdolepyg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3trdxtgnn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nzkyznpz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xrggptfp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nuiaokxd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bpjiswtb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3imgbldko.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3klkjolyn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3htljozuo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wsftzfgi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nbclryas.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zxkeaece.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yicrnrpc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xeqdvrcm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wjtyosca.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mvspsyds.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ysnylphb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bntjfnhu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iqibuskt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vnmyvpxf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qiryzhed.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3siylrbta.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nvqtzqtu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cjxxstqw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3spjufbwl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hsvsfrzr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tetwlmlq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jirdaxdu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3grvcalka.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oxipirqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3armklzze.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pnphbkxk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jdcymfww.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mlquxllu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qldmdwsm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pkkhyxyt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wgwurjao.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ohrpicly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wqpqrjjm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ftysnqnd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtvvpkgs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vlmwmlzf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pouxuawv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlohfogr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lpmrupeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axjvmlkp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wkinkptr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ctkimfre.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xelkxpyp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bmafbbwh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rncbmegw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ffillxdd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3svrbihnz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dmfvbsmm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ialijwfi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iqhmigeo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yyycepig.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rsozhzax.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jguirkrg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ylihwtqw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iuqybdda.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ntvsycbu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xrnjmejk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ltleloiw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wwxphffb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kywpsohw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jsxncwgm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpcsicnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rauserch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3owktwjau.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3goksqybe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pfoeqepk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fxqegdte.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nqvsxknc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kcqadiji.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fkldhbpg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jpxirktd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iwuxwqpa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3azwuixyz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xrextmuk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kngmrotl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxqmenpu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3adrxvhfm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdlvushq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmpucbb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3koxtattl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lshljwdg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fsfelyuh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3spzsikrp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vkmucwrk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3adwoukib.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kfaztbzz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gnmifvqr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mdiofgos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qopyhpdc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3evlqfbds.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zyyeossn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3udulodvv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zlrjcdim.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3eqofxidb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3liflligv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zjicumrx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkxxgank.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbskuilm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3oxvrztcx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfofsiqq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xowerbnd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ltbvbqlj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3popgmwrn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qviniavt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mmeacfko.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bzlnsvxr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zmgrlncx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozjzkntv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3slwhhkhy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kuqocqqy.html


<!-- 参考信息 -->