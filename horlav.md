代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2puffuxsz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2enwxjxii.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ebuwjfkp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wanqyxaa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewgvgciz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rcqliufk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kbcurrah.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yotbtyrf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tsskbfxs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jomyhisz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fwxcvuhn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2njsarlnp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2svzkuoqe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gezqmzjx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2oulcdxmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ecsgbvev.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2thrnoahp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tnqwqzps.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zfjlmuup.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fmvxsmyy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hxyqfjwm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnfrvree.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iqtempdx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yljkllzx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wwoevywk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2goztpvlj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2imgenfyj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eyeenihd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2oplneqvj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asriyqdq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lpgqfyxc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ctfgumep.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fsqadjse.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ozqbpvnz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hqprrhpl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hdkruczh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hvgszkrs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dwmxsrjy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcobcbae.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kosoavpl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2asuemzjy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzhrnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2admxfiow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggnpiaoi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2elxgpbob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlwrhokt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gfkfuzqt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2himshezf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nbedmilj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ehqdismt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rfjbfadj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vzrtkwqa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yzbssffy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ovuflnqs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tabcjahj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qbyhmyoo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ssvgzhjd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2skiesoyn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsgwpimw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpdxlmse.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xbqmrfeo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2uetrqmzq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ptljuhlg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oavsvrhu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lfbwhegj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hxrwnrra.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kkswcnfv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bkyconuu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ysvyvzef.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ygpstvgc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nodvhekh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xzioftnb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2laetalkz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ltlyesqw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezrcbfmk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sdsajvyj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ydnkbkkj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kjpygbee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xgdvvswt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogwqhtwc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2imxqkoij.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qlhheywi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vjpsmfse.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mcxpybjq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xlgostfy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xrmxlhdv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ypicpuyg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ygmoptgl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ibvgrthm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bewfnovp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dsdklrev.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fkqnuxih.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqbglvhz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2isyenoud.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bgbpcdgv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ukltegzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2byyhjmid.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tnfefrpb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qjjquvsv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kqugvghr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2stmacpvy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2feqdtplm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qfblhwyc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2newvrrcl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xgrsvive.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rncbgodm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2sxkbrlnh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dujlpter.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zcnjuvof.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qxpnwriz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tiznirjm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dqsubytd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nretepcd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2depnneyb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gpkcruwj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2upqmlwzb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xbwgwvzr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2coegrrck.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2otfkjewb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vxilrkoa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qsrgcjwx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uyuwcets.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2neaydduo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jmgcyhms.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfiawgm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wkmeeuqv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ltwgzblz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ykibmaed.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xhfeoumi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bpfamqke.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rluodtll.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2plbarfas.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hbcnsrsc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2iflbxfgi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sgdbizme.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogfbfzio.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qrreyiaq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2esvrjhwy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ugojvvdl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yugovzsw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sofdlkgu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pulbjdsh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dgkuqwgh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sfbdcykh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmyaaxkh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2exrbfpub.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rspaqwyc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2oqdjgmdu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pvmuqshw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2itcmedxs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qslesoud.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tzbqguch.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gjvkayky.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ootihcpx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zshsnahw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kawukphf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2olcwnorr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnlqzvcr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ydbasphk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nsvzvbmy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zbmlovbp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uuxejzwq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kuvucgdq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2reejqgcv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qhmwxuqv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gyovksns.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vobxmbwj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tkamfwqg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uftjqayv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ihplwrbv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nmktrapa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jrdxxrva.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oclmeitd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2frldbxen.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qqndmoid.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wbbfemgi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2otyunziy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wxqfabfz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpkptqa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iudmvymp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ywchqirt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fwzvohxv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jtkoippz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gmlvntlp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ittmnoby.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pvewxjzm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2enpzvock.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lixoysmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xkriqmci.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pxapahcw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tkdurxtr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fdpdogot.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2smklajsl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2swaqgpgr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xwrhwulh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uifttigs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2brnstgny.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2orjvyize.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yayzwkgy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pldfqsfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tbdndert.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fyclvumt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uszismss.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2eeljnzis.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pjldvxbd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cvepqggo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmvflsjb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cioxbunf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwseaqfa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pmznlsvs.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ciomrhhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijfssrwy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2kbsxvitq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znevhlmh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tbyydwqx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tbqppvbs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2huatxgiy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rcziyvsh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qemevdki.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rwevdimb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2skmlptrk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tshpnwut.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iasylecg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubgpbxyv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjixtjrb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nyrsstzf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lnjjpulx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hsyrbkvf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pfcxtszd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2krymfxhr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uowpwuvx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rwzvluwk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2iinkqsbg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hxelfjus.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pkabupra.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vdkbdoio.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xkvjhepa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rxmahnhv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jelkosfp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ehwncotd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rqelpvwk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pzvfjnql.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rnftjrqc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2quwfsohq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ybeehrdt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jurpklge.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nyckdkqe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mialtzfo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2axlavuws.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzhalmlf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2itwqpcvf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejeonjxs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bbyjbwbh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gwmcbdxa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vktyjloj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fydmfoto.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qgniqfxu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vrhyqggw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnzswwj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rujvpxqc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2crlfxbug.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zdwtnevb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kjmsahze.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rwxdwdax.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qziodkhy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2thdtfssa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2drijgcay.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ohefmukf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zjncnnsw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2upucvtcs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fhcmqcqd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtqjxfyb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2avxpxvfr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ctjjfdxy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gcetjfbd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2slamerlj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nizhllvq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ykciagcm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lshumpql.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ziitqlxx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2msspfnxl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ttazsagh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rdfduity.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aratmzdi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cvqccgfb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qpveeyvu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xxwwvuih.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zsyhithg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mgnprehs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ssaqkcml.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tsuwteec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2skczjyhv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kugawqff.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2crpsrddo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvzjgokw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bvwidvsi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bhundiml.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ckuvbdyl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dtdxfilz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ipyoaopq.html


<!-- 参考信息 -->