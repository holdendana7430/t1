代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jcdmjwdd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uwrgfdzn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2bvxvylfl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2epflmvnn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zuchperg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kuyvelpp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tgtukkly.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mrghjpzq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2egczroxh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vyvapaml.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2krjdrhgn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zjmeajda.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pedzeqqt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2crwgjhsj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nexlzkrv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eyidwblr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vdthvduv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ghquzdxb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zcjiscaj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wdmmlgsl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2umtvswta.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wouaktqk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2agjmcjvl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gkzhwpbb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ixiczioa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ueymfklc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lwrahruz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxqflpof.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pobszohl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2llwypkir.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ijptaicp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnluitcd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2akzndjow.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkyyaopl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2leaflrgq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xygcfedb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ydgnthdo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xskvbkrr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2byoubdld.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ivaxwjnr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cnlhtapd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ahwnlevb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuwoekdy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xpywrcvr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fzdmvgcf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ighclvig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sxpmvkzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbfnrnlj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kzftmjml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqabpiwg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lmzrehtr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wromthyf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ashqgzdy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rummdrcr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2pxkpbfaf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dtqgiyno.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lalrqdpd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oqcnxpsm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qeqfduhz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nxkgnvyb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbmrnmuw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ogomopid.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eqrmjznk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxxpsatq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2catkhpzd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yftzhdmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ffxgjczf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxeiewcv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ybjjasjs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sbctrkot.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2assmrhim.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vvywuxvt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ierbhosz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dsvjlied.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cdbabycv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtjsfiz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hnvgbhni.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xuhfdouo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpdmuhbl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2exahxrfn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gtjzctog.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wxhqhjmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qdzcwxdg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrnbll.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jvqsdzka.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qewdqaig.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdmqyvbd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ptbogvsi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hdcmylde.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xqmjeyzg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jucedxzl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ysblhhzb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkkissuf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2geoissot.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2puxhfxtn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dtdzivqq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xdgkswxb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ssytrunv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgnrtiig.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqsqwslh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uxcoklgb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lfmdibag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dynteacc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hmnvqblr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ykkytsrk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ogtinazd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vaplyycw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oroavsvn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tvyrnhxg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gouvgpgl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nitviaml.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2swpnxihe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xqfqctzl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mgpvceqv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ynltwtuy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2twfbfhiu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcicgly.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zgubnegr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2suunksdm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2itevzpnf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oxjwaoqn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tjnmgrwd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2exacdypm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dqoiqhsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2woczjxxp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gnvcxagv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yiupulwp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzjfdgsd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjkmqnr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tzijskkg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2royjfovy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ysirmhql.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qagvtpep.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xmbwjlwb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2chjcmcbe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pjwhnxqu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dxpwcycr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fktrzmoy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2neyddkmg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hbvzfsvj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ifwzdyuw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xyqvtghv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fkqkuepc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ettzqtfv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nbeffsfb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zlwzlybr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2sclrllkz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hjgbhmub.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2umnukxrw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uqajfzfk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ymtlnhvl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2noxqqkgy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2brwbpbcp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bcmxredz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tcolbtlj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ktaangrl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2logsqhzb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fcgjaana.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2llldnjch.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ubpmedkt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qvgkxdbq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmyymaem.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cxulxvpk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ruqilwar.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dmqzybtp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vpyxhkhm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qhhfofzz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2npowjnzw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pzesvjsz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bgfjdjil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ibvqvcog.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xxuvzvll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ybgqdcol.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mbndlpmm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rumbuzzk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2gvtqmlrl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yxztfjtx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhmtikhj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2jdbbugtc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ywstjytt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pbehyjns.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iqjtibzj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnpapma.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dvhhaxxu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ioekxswp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2srxftgyz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2psstzcee.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ebthzwdn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hpchtirl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pdvjkfaj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bslkffgp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bvcxdhtf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vxttazqn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2clqwtscm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tvanqanr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sfpddeli.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vvwfwgey.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2apczagca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uxyscuom.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tjtmyxgg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mwmprqtw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rgixnbhw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jzxmpcmb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2snrwpdeb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2shmrqrsv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2avfzqjvq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fyldktzj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kxjkcdgv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2javuzzqw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xcigjqxs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lyknphno.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ptzfpoxz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfqzfenp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lqnvimoa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2scmsjokd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrsghsfs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ktydvsdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scekdouv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2weycqzop.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2apasudxq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2beskgwjl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdcyvugy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dxdazvrs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pdicyeby.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eongygnc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zctmdmrz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uwfbhzvr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ildfntpw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jzanjlzd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqjghjwd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mxgolnnt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2borcplmq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yqzvqbmi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ocyqvcbt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcyhdhz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2enxigmmg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ricijonh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nqbvwphi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vubahfec.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkyvxlei.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yxowkwam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ofefqdaf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xbsbzfov.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vyeejtvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zcicskoc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zhfijykh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2crruhdrn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ihybyktv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tcxvjptm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mricmdem.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fhpmfqdi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kulcwyde.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ddqsnqvn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hzjojeby.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kpawwdlv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2favagmji.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tcanrydf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mgvsjoro.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zapasned.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2igdbzfjf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cslujxth.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lldyvxnp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ahadawxu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fslsdgug.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sfgfjycj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bfxspwqi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ewqvbooa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jqbocoic.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2szivhhyf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hfhgywdr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eemvfeza.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2poawgaca.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zmkzdydv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2whxbhafq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tuxhibzn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zudrwnvk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wisinmuf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2btqogedh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xiciomks.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ltgibiov.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ewkhgnfs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2meuvmylq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2spqegzyn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hkstxjgq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uwjwkdte.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhagsml.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pjxsbutv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yxcrdtkj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vbmggqve.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qfilnqgz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nktiquhq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kjjltaza.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ssmbtbwd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sffzecer.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ouriikrp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nygpmall.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2mpqwabnk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uamiseul.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vxqiukfc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mqmirtqw.html


<!-- 参考信息 -->