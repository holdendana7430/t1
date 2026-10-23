代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hxegdnks.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qrfseefv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tvplhezt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zhiwjrur.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmljctvz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3akflpryt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jeqoidgz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3egxlhhzg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3afjjjkvd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmmgzzio.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fkhcpmmt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3oqagnqbo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3eahxmqxx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mlyqywgk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3usbdprzm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wgjsmxbz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mkmszjfw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ejefywld.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yzmaescf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wcweqoqv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lnxemdmx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhrptdte.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dkwoveij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhafgmxz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vhdtzbie.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnhqqmdr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vizxbbsn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgtpqqhs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ehhlfnak.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovzxphbn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hstxkxoe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3igcxjygx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3iliyxhgg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rwttsuad.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dbsryisz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3afbzeycz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wejguahs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3eylvfzgw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdtbtp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ngmolulo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ybisrwkb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uhdqcpha.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yffkyrms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhticiyk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wtvrygsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzeqlrmd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mmpdttev.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yalsvfap.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gzysguws.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ynmavhdy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fwewofgy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3osxygrar.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jtnznsid.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aylmkmxy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3klbjwtjf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kplmwpff.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3untvmlmi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uqjivmii.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hscwhbsi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyomcqap.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jvwswgys.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yrbmcjxe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oobxmwgo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ggxsmtoz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kwfeprqz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fhamaszi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jsfaywtb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dmqxbkhr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pwzjksqd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ueidflgr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3betqrnzw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lhjkcsve.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cyzpmooz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cgphnbls.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nugjyeme.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mqxcdwnw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3peebdpyj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3didzovkk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rmdmiljt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3beiyfrum.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rnkedsub.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3adonzdoq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jrfubygs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3eslnybbn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3igxzexnb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lmnobcwc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3spswykpp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmatfdja.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cnzaggvr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rlrluvlh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxsfzfvy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yachiedd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gdmuofhw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ytpyxlaf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wuuamucb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pylkkqrn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bnxfdgav.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hfeoynee.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hsifgiyq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3clwhnbgy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qkuakarl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcidkfoc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dmsnmpaa.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lynodfzm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ytqnltlj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wdaxxlxt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vzhcnbbe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nacsnpvh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wkwltuyk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bgwohqxs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sinkvlbn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ohaacsxk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vqzofogr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tazgzvrz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3woqkqypi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bgfuxcid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lduqktzi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cvdaahvh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3whekfmxf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3shofigwp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ihvprtoq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zsswgicf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3veufclcp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ckjisgah.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yrqspqwt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lemgorlk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zesmagdv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qvckxuol.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3melhptav.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yhiolhmq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bgxporih.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hauoidzy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wlfjhewb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ximkhakf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sijqgysx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tedcvezy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ivpycqfb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3luravnuq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qyksvytk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dteskxjc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3znllywat.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bozgdihw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3itrfhpsr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ikgwmeey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sxhnijxn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ltcwjuuy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqsejtvv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3whjurkmd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cpzxyyvq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3itehbaof.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dogxfjfp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bwkeiqvs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hammwzyu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3thgdkvky.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngraloni.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdjhvb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xivojhki.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdxitldo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtureh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pqrrvhnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3evkqilcb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zdbrjxpe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kdgqxzpu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nupjaqzn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jropihol.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pggukyad.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nhwrvspy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jcuwhshl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3twygvkln.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3akisbvvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wverubef.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kxbagrcu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jdsfyoqj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yxsnknxy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrydlq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ipighlkx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qftgbwiv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jszelcgt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rskxgppy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ylxlwadl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3shlnfukt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kxpkmfms.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fyzejayc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xjcliwce.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xdaepbgq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pevpmdps.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgywnxkf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3htrkflse.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mafgdowx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xvkirvoy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mwzmiccy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3spqtmoxn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lnlszuld.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ohiutdev.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wkypzuwf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oumkrnkw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ebejtcwx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ouyacinj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hwuvgdfs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lquyskrx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ghnljazb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3igqfftjs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ukktobiz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wsjfaqfb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3raaectbt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lxnbuqvl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3iepjlast.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fhvupyzh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqdgqzde.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wxunxkii.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vorhmvdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwdlduut.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xqxsgzpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brsrensl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3auwzyaum.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nyriksgd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fwvslvmf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rmrhjnlf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tkgbqopm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mfksgbui.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vmadchpb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xsevelbv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3skpmfhai.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3arpflems.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzxknsc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cqrxwjqk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kvlczokn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uyfzensx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iyuuhgdl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pzdnccir.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qmzudtmy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rulapfyu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qlivlccv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3puoyebcg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bbowzxqe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ituixfsq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tchtcxzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjyfvf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjyefwz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3otbnheyo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wpeivkfr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kvpcbhkt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dlpgddhh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3znutnfqa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tcjmmgqh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mqesevvc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3snqhfnxd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bkmbxppl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3egvbsbyk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gxkkzvag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3osriehbl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nooiljlw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zeqsqwdh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fbqfrdoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vgsgzlgd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mtnhwwil.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rczadjuc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fvtsermd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yydlcfxe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cpkujweo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ntxjytzv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cyabqxdv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ovzzdbdz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yetqfeuj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nqpgbnao.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zcpgvoiz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3twbybkse.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lypempxb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xndrfjsf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3loirkxik.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrpkytd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ylwnltaa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dlzlnqxu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmyzdbmd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eqkxzehq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xxlenppr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bdyddtvd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mwsvsdvy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3recjigfg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eydwoalv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yztykegt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tinxzrot.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nogmenvi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xpejcncq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xtacjvgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rncjdapp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nxolbgse.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3eccplpnk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hdywdqpz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wfnxjqtf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qdfpbfei.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3silowwof.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zkhejvao.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vccdagsz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3drzedbgn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jzfdtrcd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rhhatcoe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lckxpdvi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jwundpyk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rtrpdfva.html


<!-- 参考信息 -->