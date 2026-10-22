代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pxrmhemz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tahqchew.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zwbscgca.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lnfuiayo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lqpryvsd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dbcgagts.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yxkasors.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pioafxpy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2twtrinxw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqtbwzpn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nplsgsjc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2erruldgd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2neruhfvs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dqaqfcgn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ccwyhxda.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rzkqovvh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vygklrlu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ztddlvlb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vafqious.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gwvzftcp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qkffmxzf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfmminqb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eduzrlzq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zltigtve.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aejpsbku.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svohgxuj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kpwnqqft.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alqtqadg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cxyimqjc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2noluumzy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2eldgsjbm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2awfddsrv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2coyvbdcc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kjjgbkkz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kptnjvqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bnswhlxv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kdvxiibo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kswcrlxd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwmhxtge.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ylqiwviy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vtuxmlnp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vcceycrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2uuicgwci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeddvdlh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wkofqvgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgwwivfe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lfsvxwei.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bmnvwudo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rsdxqkme.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cuvbvgvc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wadivpls.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtxiriup.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dnnovpen.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qrtjuvmv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2puhuanbh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dmqwrqmg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kcmndrwg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2aqttwtrj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2chalovva.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpuyriox.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ixjqyosl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xuglznoy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vjlplnsd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kfwpcfrf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ybtibiei.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tmwadukv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ouaabmbk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2swjgmohh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jrcgoywa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ksjlhahb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wlzdmalb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrwvtyi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tfnceiqh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2flsgovlp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fotnvjwd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jczwoadw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msznacah.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qjhfidsw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fusxells.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zckvxsfe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hzmncczx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcpzwlte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kexunfke.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2emvloxtx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2oyyduwzc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ofqmxgld.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2guckwfir.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dglterif.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqwdckhg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tldbkxje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ktnteyby.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwijxnsj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lkaeowtz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nojjxrut.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jfbxvswh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eyhvmspg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjrpiyqn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uftdetcz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpbmnlsz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ctvtpmry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fferhlwr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrwdsnad.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2znvjtttf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hfwppkyb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gazsubeb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jazmjwzj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dcpnajkb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnwovpeb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gctxqtqs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jnhxccnr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vylgpqjn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnaxwbxf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gabectkf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2spvsmnjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmdxcrvk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lbfnqnpx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yomlxfsk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kjvyvqkb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kmjcvmjv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jujhxgso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mporzygy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ccqvrxtr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tqnkfyxe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xcqfuldj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdakxaw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qwxzxljq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sjvivhty.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2imxgsxpx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2osigirry.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ubimluqe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zisqzyzb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mmmhclew.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uqmmdlhs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ccaoomoe.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltqieubl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rldgqssp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2avmbkkgz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dusdwmzn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bgrtwrkl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fvojmult.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2msslodfw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jkottgiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qqmowfuy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pnswblzr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kehzgggf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yegnncev.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2foozalwj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxyvkfku.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oebdthgl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2iiyvsrwg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dyelqaca.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xdcmcpom.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qcrkylif.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uacghmoc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2txrhpocc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kdxemflz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bdbutukk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2etqkqgvr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wvvwsukr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2anoixluf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bgoqoiqq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nrqzjrfq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dzknqwml.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kvjgfpnk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2unjkoice.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pylrjuye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lfprapjt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jrvjpleo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ovfcbzug.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wgntyxjq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pbiqdozx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ujqvqcxr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uiczpnnq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2utfgizef.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2znadnbph.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hgknlsuh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zdabntov.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2iduaqvws.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hhlsuhxi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2caowcvgx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vrnzrovg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nuveqjhv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2clfylsdk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dfhibfrf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cobchcll.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nsxftsky.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zqdogqka.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fmfhjgpj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dilerakt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ldnhgthb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2slmltzhs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gyufzyzi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2oxkbnxfl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2onzogyzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cqquhoci.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2skxdbkvy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uawenvep.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2thozylrl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lmhxkqcq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xqadvsge.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wsnfwdsx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqvcmqwl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mtagdqkn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xtjqsufs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2neypvggp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2bepmlrsg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rwzoyppc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2perdgxge.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wkgxhzqz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uvwrdqpw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ppawcmth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itapnufe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ksvkwvvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziteyvyq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mokfvzri.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2urfqmysu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mwjwcnqa.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2frphwucd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nfukamxq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mfurokhg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ljotpkif.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ekcwfodl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oquutvbh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hksizldm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvquidxu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2probgetg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gwlbcbvo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ebijsyki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gvvpkhhb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbmslq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mektzrzn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ohdlsjej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cllvfphc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tzxxdjop.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oycxynpf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ipmoydlb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ynncbzud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xenoadzb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2blhwjjpe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytcygkab.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tfbkpnkk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vzjnolug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gzuhdjea.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ccjxqars.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bbovhrno.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bhpwxnbq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wfmykgac.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vltpmqhg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2flcwgpen.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wqpgsyba.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2royjormu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfezukwm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eirbghtx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2puarlbvj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2abnigoir.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jexrhsdq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ywgyyivt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gwyjjofp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mbitxyfa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2grrqusub.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xiqdfaff.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yfhzmjlp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tmwxzjfo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fvlcetwm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2girlwvvr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iwvfazkw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nrmkasuz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fucfvxyg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lvobtwcb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2droridbg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfhvlvj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2utimaorx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2aimevyxj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhnlpulj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2delrkdie.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2absgckle.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ppsjrygf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xvpkdgvx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qjxmivvh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2perdnsnk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2edhsqxzn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mvbceoit.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fudrwjoo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jizppqhs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2amiqgfoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tusqvlny.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wfeedvhr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lxlmvpoe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2yoysxceo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zdyhvpxj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gtymfoms.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lanycqvs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xwgqqloi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yvcboxqu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gnhzwadt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2byjewcpp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pufwcgik.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ktfsxvur.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lgkofgbh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxlyeubf.html


<!-- 参考信息 -->