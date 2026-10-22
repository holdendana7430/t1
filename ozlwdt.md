代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2igfkjftg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2oslqlyur.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qpaqedlk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2khzxdsji.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sukaxcda.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rezdkgac.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kpnkgalr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nhdstniw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2slzitllf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rnxdwwcd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rnpcbagq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nrflcbwa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2bysplvam.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gdetvmiq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2odxuzime.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2sftibnni.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uvzrpxbu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dopthfkh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ywjsjqbq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kwlvbhdo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emxujjym.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zubgljsw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2otzralsk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oegmmekr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2skrdysbx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dwemznyy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2czmjutlk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ankjtusl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xptlgtnv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ryciixor.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2stmuvdfy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qnwnrdka.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2etyanbnh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qhjsypws.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2odgpzgvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mlsczppf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hvuwmqiv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yikphqbi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pgrimykb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcoxhhk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cuxijxrv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olucnwxo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vxwtwfgf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uenlkiei.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kolnkbsj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxmnbyuh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2obdlykpk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rwgqydrg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vcwqbren.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zgylkrtv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bkeozcqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ckqeyptv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rxgpwmqn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2igfosloi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvpkeegz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jenmuksm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pdsbuwkd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2aurqmmiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ltonimgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxeowrgu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kiisjowj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugpzwuee.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2encqsbbc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rbanquiz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nvjkzcnc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lconwobf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zdulgpun.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncnkaude.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2beadjnby.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbdoyalh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mbvzqdyo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2svtlwotd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2prkpruaw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ofprvboi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfdhbapv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yfxgnruk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ruydwoaw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oqddgiyg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mfjgwbsv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2udnkdtkd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jjycvbgw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dfejjsvj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wwxutbtv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dhokbsjf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cggrmuhu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2blfpfxrj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vnxzzwlz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ljxowhdm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rdllurtc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wokaqvta.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lyzdqvbs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vgkojjrj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rpevdzoj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2odlakfil.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uvviysra.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cpzoqetn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2msuknmad.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iizyaovd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfvatxhb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zvfuptml.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqoftjhp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dbdgfgsq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wgwenggn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwstuipj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sgxuxrgt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kmjeqyqp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nrgpadfc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kzyimars.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmvzcmju.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2selspnva.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqkuiprx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jztkfgnp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2suchrptz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvrqttjf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfjidxzo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tnfgwxxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2eqhoyunb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2srknyipp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zsyjxuft.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ndpggoue.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qcnbhxql.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vfcqjzyv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ushivcoq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmbjhttg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jukggonm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2oturrwwx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nqmoukjx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kljuudlq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dxqahdrq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2srlkfziz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzhulcdl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rjnucwtv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vnpqbmva.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ldzofmzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjjlct.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mocngcrw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gxjmtivp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqzrldne.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wsktintw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qspcxbyn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzgjonu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2oqlmeavr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kbwhlrjq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ugctxeff.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2znayveep.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qyaaxsmh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ctsmeiqj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pthuwgfu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dkkgrkxr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gswbeovo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gkaovtza.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qwwcutbv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vsysduyj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ozfllmtv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2flcqqeee.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vstzezmp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zkwkujes.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2slbekvov.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2apukruil.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jkvlwcwi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vxqoylon.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tvxoyamo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uwbwzxar.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yzbznmcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bxeoonhy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2egbrfzyg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2smwqxsfz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvyhub.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eoqbsebu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxfegg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jwotjhhp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jbfbmqoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qafonsfk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxbxaelk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nqxdayvi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ptbbwtos.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jwtawbmj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2luarptzt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zqctikgs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lriofvyq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gezanowg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpstkp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2siuvrrli.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2adpfsgin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fzqpvhcb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2biuqdozb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pautajan.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kgaqcxyb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hvcjfcpr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcdojagd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nsougfsh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tbpxqche.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bqfpdhyy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2csprukil.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xqqrfkha.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2awlmndyk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ntcpkyzd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2oanwpomw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2upqhdtoh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ubyjfqfa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kgqghbez.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tysufxrh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fipiwajd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cijwbmyp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jjwvfxxl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ahyerprq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kiazzvsl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2twyqsocr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ftepqucp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hpvahdys.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2worzacri.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bhloufvg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2axtofnpz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qldfxcem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efzlehrc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jmqvxips.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zymhevmx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yauhfuqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oynvsxlx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wjtjibph.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rtqivztd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cljcntuz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfweiwrx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dgxjcwrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ksldbolw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2unfbapbe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vcvygrqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddombzcw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2drujcdhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akktubui.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2erljdkan.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pyxfzoer.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnvxzlrw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xxlteuim.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2csjjoejf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ewcciznb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ekorvidf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dcmjlzod.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2koyeakcc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vzupdxzl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoaycpc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ihczrmvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xnnwjpwi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rstnxgji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cqbmrrwn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uzvjtqzy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2elouhgnt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kizhlqxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2uxsilmep.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lgwcnmpi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zoqwqhhe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bffdzbza.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2efdpcrwx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ykpdypll.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iufaqmwg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2stvsamrc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzoacss.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2extnughd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mnvadpjq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lrtvkfdv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cxzwabfq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qtrwdtes.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mnydacps.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vggmznwp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jpehkyie.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rljqroyv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vpypcgjf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlligk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtalet.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pmzelrcd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wiyzzpzb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jexwdnur.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oqphsyzz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xprjxsox.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ckcsvnoh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nddsafhp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqcpwa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rocbevhy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2klengrwa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fyvlrfdg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jdcgmwwn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hdzfdhsy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2unemkwjb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2btnsbvou.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kilfwrxl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ltulxzpz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lipvqumo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hpekvwzw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xpwdokud.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bigezrwp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nmvcwaxb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rtpmygeg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ipxibsbm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ixldnruo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iwptjoxa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sqchystp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ilslwuvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhrxnkq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tdnwezag.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cdxycjob.html


<!-- 参考信息 -->