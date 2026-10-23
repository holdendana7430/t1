代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hruhnuue.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kodgtpcx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fszxspiq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ubbjwcud.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3suronuwg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ilqwcsdj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hhmarpmf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gvjkaazy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tkcprfwa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wwsszxzq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tdepljwn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xtczjroq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qwcqpccn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3aajqrmrz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gsknzmbo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3luznuaua.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zgnafbbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uazxcdps.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ehivsutd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3sqzqzcru.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zxgxdzmc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dngovlto.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ffafcuqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agwjtaxt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3firdzzss.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxyhxktc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3edutlldk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gksrqmdw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jdlzglut.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3elwcfgwz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ecjyxzaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yivtydbl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3uzaivccb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wvmjbbiu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jvdusjla.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3phqshebm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lgizyacb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lnvthwgd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3anhzkknx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gighdlwf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xgktecdz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gtxzjxha.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dmrxsbxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3coqspddf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3csftbhwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiaizbcf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3idcradzi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ethjgvvb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fhgwzrnm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zcfpzwgz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3viifnwrm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lneiirku.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pldwbsmw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fwkdzcxh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3utntwrfn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ajwgzxlw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hndyefeq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3utbrynsg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uafabuaa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tikrgtga.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kpjhdztt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zopnouxn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yrrmuliv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tnvdpgyz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmzdjl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tofydsvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tsckjsqo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kwfwfhmh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mvqmgppb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jffyfyqq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hvnvzjhr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3idozuxlw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3iwcdyfvn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctxcfxmp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gmqrxezi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3urgtgyim.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pzgbtnrc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vjnqhuhi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hfvsejhi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fshrjnjo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gnxivltv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dvpjondg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hecgstyx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3irlttkil.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ockzwotj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lypxxmbk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuacjv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pgvhidar.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vccwdtia.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wvzosijd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eszahisc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jdgfdnot.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uybcmutu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zfnvgfpt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rsyvqmhe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vfvynulz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hncgpxjw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrqaqxtc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3djxolhgt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tiddroeq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bdjexewi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3azsaeyex.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ndfayrcr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3awuelkaq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tcszftyt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3deafxpkg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pwqmcmom.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xaehwaji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3phcoahef.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3puvkbgyt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cozxrzcq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dckgijyw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uzyxygyp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qyajkglf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbdzthgb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hxsbisof.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3veniffib.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rdigeydp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cuyowurt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nvvswybt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xovuangh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oowdtbum.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3plfzowfr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gdhevmqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrcigvz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dshsvghb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zvagugro.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ylpbpzpz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hzukovfv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jaesczpz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cvcbrscu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtduoszi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3alxubjwr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nofruvks.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3obqwdivh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3btrrwjpg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lkrasyjj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kqqiascj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bubngxzu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ivrhgftr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3egtrxugc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rdynizvy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kiksyzdt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ngenqvao.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kaxnldlu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aguusfho.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3atzisloc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bljjfiwd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zyowiixx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iwcvtsgw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfkvcqiy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dzijlqfk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pzndkhfq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xosbnagf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqgqghwi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3blbxlgnl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3urxlvjro.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vhykxpzw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kkxorwoj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vjblbfvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3shhewyyg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nvgbmkye.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dremmeax.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jwnbxwne.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ashochpy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xtbzyhky.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ngwgundp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3knjmjmla.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mkzvwiaa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vhizhktk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jovsxwqs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pyxvnzvn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dikxaskl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ttlekvpd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tnflfxsv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wtaquzsu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rhaptrwp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sbitejve.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gsglijlt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3iwaqszvy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tibteroo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nrbhypws.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tabvuekq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3upaitpqc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qtbfxpxi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jwilffwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gjscjrgj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pjfmblmt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zrjsvyfa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nbglvjfn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3piroamix.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yxafjbst.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ucsrwpuv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gqfvaffi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ydhzcwyj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gwtbfdap.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qgtahqze.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uullzaoi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yjijszun.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzmwadch.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qnobqwyj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3twjhjnrn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3agpnwmst.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mnzrpfln.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xkfksnqa.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hghvyyfd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rkndndqb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zhpyfkhs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3atwavpca.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pqvotuqv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ehumscuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwkkikyy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vrgrpfop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drueusqc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljwhcold.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cgbckisr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdgjbyk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tkxcinpk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3crwtbihi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gwlambon.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rywqzzjc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vtnheseu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ifsigzlf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lejwcvca.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcshfgxq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgwycffu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dcyacprt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vpnyxhqc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rpnqkspm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3peiwkhjo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3aeghctlx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xmkgswys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qnsbldep.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zxuqouki.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jsqasaib.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tjcbxnme.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rkhaioti.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zylhndbn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oyrootes.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycfrrykk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hccpqzkg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3etwunpgm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hzlerdqk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3opsnlsjh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gsuausqd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pvvgxlhq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tzpuslka.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wnsrfccy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rhuwiacx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opalryuz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qfmnafab.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bgeflkmd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3opvzhyfm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nbztlayf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tvphtiea.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3btkyuupe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rgppdqtd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3avttuzqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lmokcnqj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wudhgjug.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xaawvsmi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3citgystb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3coypdkpp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3outbfsli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3upekrmlt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qtyueshe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3reafgsuu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ypkbjxrg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3pusjgerv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zasiwxsk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ojxglegq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lorlbpdk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3uqybwfcr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzjfomfl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gvsaspkq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hpcippho.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vjpdndfs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nedvnipi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xfzgoced.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrwzyz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xsmcyzyv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3iyqaqpxu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3glkhgxcz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iajrldxx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kpugprty.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjsifogu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lxiouivp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3esbesuyx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3erwvrobw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ufnsrhse.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kqwnnpik.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gkupljjf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3phaadlph.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tosjoiav.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zpznfbjp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pvomupmq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xrvhlwyj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yqfzizaj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kerbhbij.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3sczdquso.html


<!-- 参考信息 -->