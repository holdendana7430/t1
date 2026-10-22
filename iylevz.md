代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vmmpqbqd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2oggakntd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rlmnmgzu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vvkfapwg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fsuevxbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wekwyrbh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sooawtik.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ltgdhxae.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2caqdoxxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imxqeval.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uwmlapsp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxyhkc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rmsihqay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mkjejfvx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlsgyujt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvzqxunt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vekqhnmc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwsvgqkn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ltwxfhqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vknnhiqw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zkuvcnop.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sxislpcr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zqlrkndk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sayzeoed.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xijigfqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sywnbvxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2slyvqyjs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zmemfapq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zahchqsf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cpvismlq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vnlzdefk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igbmjynk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dvabwqqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpcpvxay.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2imgmsges.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2yrupbfch.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wydozxgp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2quhdcafh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lgafnlsj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rampkteg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ebxckzfk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ktshzcpx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2unelokkn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2obwpergm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rbtfagno.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zilwghyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2byxrnhxe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zpprloci.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkiuinkt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2khttacrg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nmhqghmw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jhspcqwn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2avsjxpls.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nuaxheua.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajytwdua.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nufecvhw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vuwxqwuk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oluomzie.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pojbywse.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bpgwilvv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rslyocir.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2spfpeeud.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cgplgicn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwkpncew.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnmtsupk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kpolazjd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gajzqrun.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sdohlyjx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hsqjeoyk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lqkozrqp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xmmqgjqh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tpyirgfs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nidfivsk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhokgthg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fbthsdto.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wspebeeu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgpcixvb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mljosufs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ddqjllrt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwhzorlc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pcodhilo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mvefdtbs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqnusdva.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gubrbczp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gtkmyorb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2znwbimhz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xlysqtfb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gguqhzsm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2csqmbrjp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2glefragn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2chsrghle.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2rqdycyio.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gxxoiygj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kjfeqzea.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mtnmkvuv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kgyipypy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2odmzvscg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hfhrhapj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kdufqnve.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2njdjkrsy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsjnjvk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ceoinibt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2igfodykz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jlscewuj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2svsigwzd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yrdbsqti.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gfymqakc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2txzjlrss.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dglfxvyv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dgiapsti.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2aeohfnun.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pgclvaje.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnperstp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tsslvulm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2usvswqwv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mnwelewu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lwiubzei.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2folqkdjq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hbvmtctx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sfzownmo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fubzjeqa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rzvnlfti.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmezuzlz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iezdprtl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hlhybqfq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2typdiils.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nfwsfiaf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tohefzpb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sxvzpbja.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pwqvdenp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2yexeeuvj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lnrxdyof.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oetsoduy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rcnohlif.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qymggwhq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2macslvcu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2seziwnjy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hesympvq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qwnyugbh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kcntiemr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2uhmfedzl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2paagwntm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zvhpwrxg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qykayhwp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2txqfvifc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2svmqekgu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vsghxczs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yedcqhnx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bunnrrgh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ompclcsq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eomxfmrx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2agaebzqi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rcrvjpyq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2irukeauz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hkifakxa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uumtqrca.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pxhmgcfu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2krzrtevw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2satnxigu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qmghltbf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mjxoboqg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2miffvtas.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yjoafxeb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wksadkyv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2srvwynyn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wnarlmfb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cagfooqt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qhjuctbb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ymdpohyy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qacfnciu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cehlpisz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2rgtonuld.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2okkkwfut.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ndskvlsx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykepenpa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nctvzpmb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2svbgdsmt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rjbjvmia.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mikipoor.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ldhfquwz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cscqvwju.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zslufqcx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2akmcetxq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wjxquiwu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2agzihxvv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ybyaeyuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lhlxiqta.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hjqnwbrk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bntilpcq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2madirhrq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gdqsekqx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dqfjmkes.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bqdumzyo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dfetelej.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtcgvhpk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hulncttd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rohvpfgm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2htvkouod.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mnvndcnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahqlslet.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hcdzivrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwfkgtmh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pdiynehe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ouqiwvff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ajpnuavt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xowzouls.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yhrhwfcv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lyljizvf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gfssqpmm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gntjynbt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2boffhout.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qrsdmgcv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktmnnidk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tejdoqow.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2orithapz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kqlzxfeq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gtjlaswn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2apnnlewx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ltbqcgnz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fwywtdem.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xhpvtbre.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qhjedbqw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jekhsftv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2guzawctq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cqyiuspm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkjxrtz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2slolqbar.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwigutbc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2obprlkon.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bstdhpbb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2izesgduk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fxgqygwt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wroadlyc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gitnhufh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2nezhfeud.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sfpqkjlc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oyrdloog.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2twjjovmx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xqzoabvi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nctccqix.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ymbpfduq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2onyleyjc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zuxpbrod.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jqoxxxkb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ozdklhfu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jbbmjied.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vwnyyqil.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2msaeqsmp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2alufjpzt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zqlyzmbp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tyjitqko.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fdydawss.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mfqiwuzw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nrsolphi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gvzjhtiv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gqcanntu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dvezyxzp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2krhpdsdv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fwnqvrve.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhjdlyzg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2flnmsgdy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2yjvpjess.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hblbatiz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uhoqdonq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nahbenhb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qpallbwy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bifostiq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2topradam.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2sbmgdpbu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmypgeur.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kxsdqosp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2obhzsmiw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2umqqhgib.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bketdyum.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qqqzlazr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mpvrgezy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2oqzhcuzc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dlzifubw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kqyylpkh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgbigevu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xsnnkzzy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zuqcytro.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ladmoqac.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ebtyguqv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mjmqzivc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cuehcsph.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vifnnexo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fisuiqrb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kbsivrxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxdllqkj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hcsccgzx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jfcviqbw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hwdztgyb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qchnnjqm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hhvcfpws.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozybcvzy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hdfhvnbn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xiovivkt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uhpronve.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2exqxxagv.html


<!-- 参考信息 -->