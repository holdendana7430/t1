代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jmlfbccc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zunbkorb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nuvryaev.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uosrsjzf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oyesgrgf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2izwiuucw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rtyyrzfv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2plzezppq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nqxqifkj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dxujuwrr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yhuegpnv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zibteggb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2uzazgwgk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jlynnxqu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kpzjcmva.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nbxliydx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2swhjesjz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vwmmsgyp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2asciwcwi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mvpdnaru.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kmwnjrwy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qosuacox.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fhuwfiwl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vothgxtp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xooxydgx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pzrhlqob.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rlqusoun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnvvxtdz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gkdmnwkw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtezuoqo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2maupzqtg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2axrjvxfv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fwwbgpto.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vknrflff.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lokfrfvm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2iwjdkwin.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tzypxjjk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qwehqtin.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sazokasf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hupukiwp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qjporiow.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hipievry.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qkqsjuir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxloialm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rjijrwhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhkomfxe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ynmrnhyx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wyjmeuag.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xacvxafj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vgmspyak.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bfzxaoqr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ryucynuh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2kdwojgsc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqtppucg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mvxbpnuw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zujnypbd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tlokocvg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eaudwjfq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2unugysek.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nqmqlpvt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dnznqpfl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eoeyadao.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qrnzozqe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vdfbhfbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmaxivgi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kojpprsa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjsiyb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qessxhme.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ciravgtm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ynsfxqpm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aexicmts.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zhfcyjys.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tnfucfca.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zkdkmwev.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qgabxzwl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qzmibdml.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kenusyei.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2luksiocf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kaanhwpc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewpoxjke.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qrdhxuoz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2doqarfcf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tvqogmiq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zhchddby.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yuhhsrii.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2egijllxa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2puofyrgx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wphaftyj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2embdmnhu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kdaecxrk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwobyoze.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hozwfzbs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jeltipre.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ycxoqokh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2okofudgx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2omrbcvil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ueiyqrbk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mjapnrhg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yjdyoipy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tenlalfm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2asujvslb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2uzbkjmmk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lzbnjnrm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tunqutqh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ceawfowf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tgctmzek.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ltkbxruj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctumtxrx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfkskeaz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tqkukrkz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2eshukxqn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2sligcdtt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nijbbzxc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sfpvkiml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2louduixs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ochfsoov.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qnfafjdw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lyrksjjn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ogmryzug.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pvxhwekg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2shehjdkm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kgustqxh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bmevfamh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bqcebnsk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cppglnvv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gjddqyyp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pgzlpovl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pjexgkat.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ssalzuuc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pgfddsjh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ewjrqrlf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ijxfqhcq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ackbqtaw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hyyfupco.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abhtcmpt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qipnxekd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xvtjersh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ddudjvxt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iqhndtxm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2pxijuuco.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2khqbbfvt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nzcpddhc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cujhsgkn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2idatgzgd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pqyoeqgh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dgkctfdw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2miwgmruj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vdfppjaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tudlalil.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xzkzguxe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dzftddcg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nofihmtd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2oijjjyfh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2lglteimu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ysklznfv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mdfraect.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gyzmulmo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2atimuyqg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rwutooqs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2uyetyfca.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ruicxvms.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gklpfbjl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vfhlzqiq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2afthxhvy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2batexlzh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgcfetfs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wfuebjss.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zmkqpzlq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hebcyseu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sayihynp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mduzomjw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2eqfcmvmk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2eozvrirt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hinobydp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2njivtved.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fsnixlid.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fjibratn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bvxcsmnn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2eokdkvkq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sbbuzxys.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zlbkxxrd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xiuqguuv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wgixhkqh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mfimwrza.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2siwanktl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zaifdkrv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2notfpych.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ruovhyod.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2muefaeiz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pjjlkxno.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vxefvwxa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dzhflpkq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kjxcmjip.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2feowjcmo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjirobec.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vcqbofqc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nrupgbon.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2obhehlmi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewlxdjhq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngwubnlw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jagcddel.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fuijprac.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ubtlhgrq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xsdznlvt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rmeomdas.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lfynmiek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2baximhgn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2asqsuhwe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rotnagbk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fvoxazsc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2itdzyxka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxtskyob.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wbyguxxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivmqhofs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oalugbju.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2orufhmqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtgeqblo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zmtkqagp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yjoqmlim.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bvlhmhqd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2plchxfkd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zvjuvskt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xrpybaeo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jqbumhgh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkccslhh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dwxmzosn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xmmldhxe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wtolsxgs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lanfdhse.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lixhkbtu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rxvawuyo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kedelwao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pejbwtpw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2aivreoef.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zpizctsv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2swdrnkxj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dgjcsutg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uuuenpkd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jrumuqhx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bpavgjcl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2taczcuyl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ymsdhyux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2yrifmesa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2beqbxmgc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ulvcofwc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gmllqkvk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uernmjsk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pzawioyd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yteoehmw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2usxidgwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2raovsfzs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2etbhmoco.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wgnmrxzf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2elwokdhx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wbhufwpa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mgrxwemt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uddxcrma.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2aewcdnht.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxstvnl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sunugitr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zbnlxdxl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yhkkjxjy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rxvqpish.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gxsnhmij.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ggvlanpl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sttpgpsn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nqujmhuu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cxwownfq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ytuadocg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lasstshx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ctvzfqip.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lyvlzzei.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fovvcodc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rbnmases.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vlhkckkw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xtilyimx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kfynvvru.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gnyykxhg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvvwiq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vxnbirhy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2oxiviyca.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pybojzgk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dyjiuqtp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qdphfshk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xxckanny.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vqhxqgbb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lsxaltsx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsgyzad.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zxixcbdr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tytlofnl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fumfuqwo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgznjnpq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2akerybmz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2naalhzbz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rurvrvcu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gwxszrhh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wimztwrn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zexvrloz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2auqlvxra.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rsjffewn.html


<!-- 参考信息 -->