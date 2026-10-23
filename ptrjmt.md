代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vajfrjpv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xummxklh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xgngawcy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mesqlpyf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pmcirwhz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xdeqqudn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ygvospyr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ragywefn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3critxzpy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wnegguce.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3emshoxgt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hdebqbfq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bfqixdwf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zctnyzxz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hvbxoxhd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3aavfsdvw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bfcdiakl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgqnilqu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wvmralnr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hoobexla.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ibfdogeq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hhpgnfpt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgykacog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtsvdopc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3iansuebq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3osmlrjem.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3uyjgtimo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ztbbvcwq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pafgcqiu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3msvncdyn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cuhlxqzh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3unltzysm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tsmzyvms.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jfppznqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bcionzkg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3cxtffqry.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oguiwuzj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ptqbewmw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3btpyejhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqqevsbd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jbtuorgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqzlkapx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3paqfgxgt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bssqjzpb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3eoslvrvl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pfgjaonb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhmvjb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxaqcb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dwnrngia.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3thlfchue.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rrdtgmpo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ixvxafwm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qdjgxxjb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sgvgrhgk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ejzkadut.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xubcoazg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3upqniqlc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mxyqhtth.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smdrzsnk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wtjqfmfo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3eegybenx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pbtmvygy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3spbdpwzx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fhkvhefw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3oaspjsto.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mryfdfca.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3clhvdwwf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3igidkcgm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxofcu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bcjtddhe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlomxamr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bslctpla.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uteewhzp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ymgxbaub.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3klkfoqnc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yclvfskf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yncvsupk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ywpnhjtk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnigsccp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3heqvcilq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgfwaxsw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wmmyneda.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ilbkjnxy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sfzcisey.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nyooekrr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ximuzeqw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qarbkhka.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3seltddjw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcnacpay.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sfyknypf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mftuiuvg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bqoejbgg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bwprgbad.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jqralgwv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nejbpuzz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xbbldjqu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vlstutqw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gfqzurcj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xawjneod.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dxukbhhc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3htzlfcik.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lndkagrh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ztpuyoto.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mrucrwsi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vakimriy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jikrsoxu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rqngypfn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mudmjrhz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chdxrndg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fwwrgkol.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qceqhoek.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hhbjjqxi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fnvfzryt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dyhbdwnr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fjhllikf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fcuxwhyc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fylmcdbj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3itbaejqg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3spygnmig.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3myifszsp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ziarchiq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sxdltlik.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ytjcwpvu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yacyljlb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wkdjifrr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ygysvwpq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tpviajxv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dvgovgqd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xcehkjip.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tjwdwyyf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkklivfg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqxptpac.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hkjoffbg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mzpcecas.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qqotaqtc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3orbcbwap.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vqtzrgov.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dkfktpje.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dnnbfrkq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rdzhfson.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zxnwpgzn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nfsijkwo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hvagpaqa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xtusjcte.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lldpditp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gbfprgpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mrjlusqw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3usatwrym.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gnaztmiw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xwvsubfd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lpohrqtt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rdzrjfib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qbojnkii.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpoymnlk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmqysn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xxvvzyss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ukyolrup.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wttzkxel.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3odveldty.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uwqhqjno.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ecjrzvkj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ihnxybns.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ljrjiesw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xzilepjm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3psbjqwhg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ctftvpyc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dsptamzk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hgorafvk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jrkhixnq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xjmpylex.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qwscdbro.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zcctdjdd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3uzbztfgd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kpkigfaf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpylkor.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nxebqahr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3peibfirt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3iirdhhty.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nxpujdkr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ldjdlcip.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zevogzrg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bltrnwcu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vpaxqebo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fpqngiqr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3btypfakk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jxqmofqf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ppzvifdf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yjodfwqr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vkeyiszr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vsniolgf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pfduybnm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bnwdnqfb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xipyqjce.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xcttgops.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyhxtipn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oamoktry.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rcfwnscq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xdwccami.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wpswqhvd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mvboajrz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kdgvdono.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pnmpbxdl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3aubejpve.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3afyjbvwy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cvrsflnz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xwaopvne.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ggfzgpdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahqgqtjm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3orrddavk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iivswuiu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlnqqtcv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bixjzhdb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3twgpplza.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3frqdrbvr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvliijf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vftcgjfv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3thzlfweq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jbyvahaa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3osjebbjc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fiqopabw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tzhdensp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pnzevvnk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vgaeynqt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bagkycxk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ugyzpykw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uzommgci.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ffwcfipa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dzgvhtll.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dkekhbcc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ypvkzrxd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3opgrtpww.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3easjnzzx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tukgasnt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3sbhdwlwk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nqhmvqyx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxihgyne.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kfrffcem.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jnlxzepy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ypngzoil.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ucbiriwv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bmpbujld.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3etbpglfk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pglhwtbr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iiqgeizk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hsofwryn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ezzpefqy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fgnijcdl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljosycdx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ozssrija.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fzvgubkj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xwqsifia.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mwbcmvzv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xkolxcpa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hgklrqvf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rmnsknwj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3otdqwkgs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zjemecrs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3udtyrbio.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vewcdtut.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3weydujum.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3latzuzfk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvowql.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nvavehqj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fsexpxez.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uhldzxlx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bwtyuxwu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwacktjv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3grmhndjf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xrmzwdqd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxowjope.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vlkldapj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ajmaowbh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pdzajuif.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dscoqsep.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dbzycyvy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ithkdotc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3murzakgq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mfjttzaf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kmxwizsl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3klwcuzzv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ixwqmqpl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gturkrtb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oujacahm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bapdxpjs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cudpqabu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxsxnwqx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kqjlsxev.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rgvlmncj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mnhhqyon.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpoylnye.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgcsjmlg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qywhgmnm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3svtabyri.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ljqipksc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zhawfdmn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3duzpsczg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3okmjnjwa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wczduwsn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dwnuaskp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3znvkrhgj.html


<!-- 参考信息 -->