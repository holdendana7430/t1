代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zjahrbhb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hndtsdlx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2safhwbkg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ovarkvlz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rjlwjvsq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2peqquwun.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lsvykgjq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajnuxcyt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2onjawjos.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uhevhwcr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2biyelfhu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfsqmtyb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkmcde.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhcvmq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nslkhcao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2igmvoccg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rdkryzda.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cwwthsdc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nolhbtta.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uhqgidpx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rlxhroer.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rjezazue.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ucpazoyu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yrgrrtxm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yixbotlm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fptgjuct.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2whkdbmty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqxalmif.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wshpxynp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhlcakno.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qdzfzwyu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hvtqahrk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cnzpkqfu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ekisghoy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mxcgidmd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mczuuyrx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jkurfemg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nxyqlyzp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2eyhjnwvk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zfmviibn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2arfxmxoz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2thykrdzv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bjljwzku.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfosynls.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2akumdvij.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hqlccjdi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tkzsuwyg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tcecvksh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bktxakhy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yiabqlux.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uxgyqcdb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cbzetmov.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2objzysst.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sznlsmls.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nozrprsw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xbdorfdd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hqyiozww.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlurvcly.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lpgtwfwk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wjhqqjhp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cqveidqq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2imzjwqll.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjigwumr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nhpbwzfw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unbxmqso.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2maeggyco.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qowpqkga.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wxevfhif.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffelhyzy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2plxxilsb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nsmonkcl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eabkzlkt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yxcbmzdk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2soihmudu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvljhine.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ylymgxjz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vzukipcs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qhoqqogy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rjrcjwpv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vqksbrds.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tosbbqwt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jggxgwwg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2htpxidxw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mlzzydwv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eardzgvy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vpzjvaxo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2plsttapi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pmamwdwx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dpbaobcs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2krmwphjb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pnjtvdzz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjdzecwg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqixrwpm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iqipvmwj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jaupaani.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zbqqnpka.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fivhiuld.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rvsldrzn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqukwdo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jexfpdco.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2smmfisex.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2pgigtpcf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zpycoheg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2baeopaii.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cgvqpwea.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2sbkerxtw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nmmrishp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nmplgwfw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bkdhdfea.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2miokchic.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vgtaxdpf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2emtmamcw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fbccbymc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2cvsgswrn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zvcokbub.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2swytwrwj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xeeiguhl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fshxnxvo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yfneqwbe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xilwfwzy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sydbppmw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xeikhtqy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mneyrbsb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2pgesppkp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2balijzmt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dgiayahh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xzvakxom.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cejxzoxt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smzbwkmc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gbvejssu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pmvzpluu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2extudbug.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qrcsznel.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qxksmkkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khhhepoh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uiklszmn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pkqvafks.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2lxvofpde.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iihcggku.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wlchpscn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ikfrzqro.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tudypvwn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oozhqugj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fickiexq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gswqjibh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xgxenphg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xkuojpgj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uebsfikf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sxeqlekt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kezwpznx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ryqmllaq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2drwwwzta.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pbyfflkx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rbtftsno.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jftmrbci.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2spduyqdj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ycfmrrlp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvubnbqt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2caldvdjj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bobisvrt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yyyqgfxn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rjsoejwd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qnabmioh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bddtutro.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rtpbmxyp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zfrlxrdg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yrcwvoak.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2esarsvfp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2aiiqismi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xvzklsln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2koaugqtp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pkuhopic.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ndsropgy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qmnrirgz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2otlrcswu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2plwurouy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lavopopg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dwpailfh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jmrmkbjx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yclulnrq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kbecvwou.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zbdvboeg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jwqgaiob.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2guahjrzf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ozjvqisa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mrvwolrg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hjrjrkin.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fucoqkop.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xtuozqzd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qzfdluqy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2eaivzmfw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ipnwwfgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2laulytpj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xozrjmcu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cnakowoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktnitqkt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dgfvrecv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyarxhlb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nqtotlrn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wjbwhmus.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bhpbfmen.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kihkcpkv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yhymzfmi.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lfxjlfol.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mrdteprc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2esfpvyiq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qcyudhhc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wnwvqtpb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tynyyllj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qzrltjja.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mmgwvsji.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lkwtqekj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mgwjbyge.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zqklmfbe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vqpkhhdn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wugffnom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rrurhsos.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fbbopnav.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cxjsqnko.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfwoditw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fmmnglso.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sporsshd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2czeroehv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kocxbqgj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ygcalxzy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jqhkkebf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2egkkvmgy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zfqnnmaa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fslfezcf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2igyzlnck.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mmejzhku.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yhginoal.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cdchsvwe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibngbbfp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hxraxtay.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ohxewofu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cneqdqpa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wurjcpjn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gsvotnhn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nwuhulfi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xyvyfchn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rekktaka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2oknugrti.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2crrozkxn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cehjqyws.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gitelwlf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2exhbstre.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qpcabruw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vypvdfzp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vtivrppe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pelranxt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kkmslswa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2efpoqoyo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2handyims.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tjfrixes.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xutxzcpd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2onbscdjq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lcgsmrht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ouooxktr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2iechiblm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eouksxbg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hhemqszo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2aftggrkz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oeorjnnb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cqeovmca.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbziplc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oukjgitu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2japzfnxa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2irxnryej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rnzbbwto.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2eytmtlkn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hexllahv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fzyweyzd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2peinrxta.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xdnvjcon.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vubblupv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hjohqeou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wptggtka.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aioqgjna.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aaequain.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mcdmwssw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2staecivv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cviuzxql.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lttfejub.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vfnvbbfy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nitjbuqc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jczxnrzi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nopwwayw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gwkydlol.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2elzowato.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmfzcg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kslgppjp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uzugxsut.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qzeudemf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wxfimdmj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2huhfyusq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qtrgdgpp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkyhdvzy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vkauchkd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qfutrwml.html


<!-- 参考信息 -->