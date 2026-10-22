代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jkjujmps.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nnlhkzgd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2sykzcxec.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qthtoqzi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2bxvwrmrb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vrxkrdcr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ryrdndxt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nkysqzsb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2njxnapwq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqoteo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zkwacunl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xfloljmo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkfzgztx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2shwwbbcd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rfsrgvmj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2huelbycd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yjlalggh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yqtonxzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cawbxnji.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kwamdasv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2awrlqubt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mbinoqgt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nbamnhvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2czbujxuf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wtkwibfl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sbdtsdja.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ydkmdodp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2skqcdplv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tisthwjc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtrlexrd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ngdcisdy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxzwqnoz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcuffzok.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oztpvmwd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sitqnvfm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yqbntvfy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ohgmniwx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2egdkugav.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pilfvpsm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tnxwyawp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2nbizvpjs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vuoqlbbf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zjvfyufm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2achhayvf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vixjgwdy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cwbnwfnu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yamrzcdh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tujaiqyn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kibkaliw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ylrxcjpo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ibetfcwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unjkdhoh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2etudkhju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkxmyjwt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2eaxroqhf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jsamnboy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2srsczjsz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xuilirqt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dlykmbzl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qzfmmkaz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rftyrasa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzpvzsyl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2onchtqyo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rcvzudbe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wwvkeydk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tljpludm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpvqdbrs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hgrhject.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jgqzejvi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lkbbgxgc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iewztvsn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dejtgsyp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2afrogrkt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gknmcame.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vbakvcbv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gvvksbvy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fibaftwb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kkyvfvvp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gloqqbvj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwwvopfs.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jhoaqoas.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bdyorxvj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rlsvrtyz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhxoiskg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2komffpko.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2duuwlbnl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mobtimvk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uknfasld.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dsmdcime.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zapjpdkc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ferahabn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rzbdeuaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mnmoyfkq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ftobjtsc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ychcnwvk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xvnirrrs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfdfpfuw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xtsdaekp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qeiaxslc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2alsqprde.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sprkbcxq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2deejonfy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqrjukto.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2phgimdgl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2whycxnai.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzkcvqbo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pqqesxfh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2uafumynw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2evodozhu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dqzhkrua.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pnellzli.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ydsudust.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zfepfosk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ghbruhrw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2weatcvwz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2juqcofll.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lafannyn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vuvugdkx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2assfuhxh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ujbkpndp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubnaaohb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2awulijup.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzxhahrn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gdjfjqup.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dvugldph.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2edyybgov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eqgkbhwo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2oykdvjtg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ecfqfldr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2irdaffzc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fhvllkgi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2aokvtprj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lkifatsz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jnopycbp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2szlyeidi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cuikavrv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2egljbduj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xgnonzsn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bvlurtzv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2msdzvxcm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fqoweysg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yjlvinii.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2liizuqch.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2utrhqkuh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dkmvdmtj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lrxwqwwm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dacypsav.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xralbmsy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ihofkvsd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ilnsfumh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ahztbmdu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2azxuaqvh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2srgxwvok.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bcwlfudd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2psfqqcpx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2quvyqfjr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nmyghcgo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mvckjcpc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eluzlyhe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cfatvcjh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yvrecfsx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vtettqhw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsruyhhf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wnaanevw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2awgyscxi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2omvyuftr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2chkkuerv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2anrflblh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2izvlmlfm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dqnomnnh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wzmavfis.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2couvoebo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bhgeyviz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2csrxzwqb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vhymdige.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bphnmtxl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qrpyszya.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bnckcsip.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zncdbqyj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nnammivu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2usjlgwjp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2atcnmibs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yqhqhdrf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lmtoepzu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xetghhad.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mdeboavr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2punhpmqy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2osqjvpno.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cffxsofj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xwtnpzor.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uuctjumv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wvzhizum.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fwvbfqll.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yshmidxe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tntcbewy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2slibepkw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dcsngnbt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kwovqihh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pbgfmljp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ifgptrhh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rrqmhfll.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jpqmhjgk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uhkznvrs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2noiyxuoi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2umswhyly.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cqopptqp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zqmevvqu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dspldrqo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zkrzmlcj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2eteoeaev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xmnfzifm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sdclouju.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qhoscxqx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2onjgqhtr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tkadyobc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ylcjqrgo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwqnhhlf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2kkhercae.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tfoomtri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opqljtos.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vxfiqrxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogtaiaju.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zjiaiuge.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2itnypsxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ihxpusuj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nmdyhvgg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rdazitfs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vmnbqocf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gshechky.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2riqkyyfe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wamlbmtf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hinblkgk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ofysfgqx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rsyxigjz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2srvpblol.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2njaisnck.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wuqfewur.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ddmambkk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jmeggxmo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sfdhpnau.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jtuvvxdt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cveelawo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wmtueelx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xvygtoqe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rphkijrv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jtmgtrkh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2prpcxeal.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2byabejvo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2apjdheda.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tmlyosfv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sdxpodjq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2voteuftn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xflswrvq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ewgdxueg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2iipfrahq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2njbcskim.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bfuneepa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llqxkmif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bemdiwcf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lkavgknb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2eigriamd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xnodplrz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xtyjtque.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2acxxkhbf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hxjblcse.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fuvhxaor.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zgtgexxw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xogxizzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2drxgaums.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sasfjhsa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2drxinchh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lfdrzsrl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2uzklsjru.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dpopihee.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rzlnlycr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tlvdmtwo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zunzpbum.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kqoogued.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2klfggcpo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltoomnpo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sngcsxdc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2biahfmap.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bjnfckeq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2webxypbq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2frzzoecj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2geknwpzj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kfvqygvz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vdxncxjh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kakjzesr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2sntzlnrz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mjxcpfez.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ulpmqxbi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2necdobdl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2okilbzce.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2whuvzxij.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qiqyhbpg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gjflyuxz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzclopr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2aikkngrr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kuhfcakt.html


<!-- 参考信息 -->