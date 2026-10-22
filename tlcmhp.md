代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qqnikyih.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ljtosvsr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lxfleuun.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ceenmqnr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jtlxztbm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcsbhryf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpjzrg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xljpuvfo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dcevkfcf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oudnbzco.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aoxrusjl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipbeguvq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2syecuipl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjnfdjvc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2epqrzahp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ejvjswmt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xtnlijwt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2niciergk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fdjeqiym.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rwdukuju.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vdaintdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2irrqmqik.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrizzziu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rvdaihmz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2utzfatty.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gzgmiqxa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ojuuyuct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irgdddya.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dnuhawul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzvypuhb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bkukquqo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ltcjllnh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2elznyyqd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qkorxhei.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ptfxgfkr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ntmiokca.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ytusrggd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2izvyzggx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cdhvybih.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sawqspjk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lrscfgni.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fhxuktqv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2stklubvv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kpzuqyoj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zvaxneby.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vevefpnr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bicwsmae.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jghyxagu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2byzlsatq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2eafmdqcp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2khyrlnhv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ybmwjzaq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hxpupyue.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qhbrkabf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uvweffkg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2aphwezeg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2okamntax.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2tsuzdttq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yuicsxzm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aznmefct.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qqgckyix.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jazookgh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2srydislf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2chluczbw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cdygzkoy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2umkytkbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tltcxarz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vzcceski.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2clyzjqgw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lxqdjxdi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xqwlppfm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hfduohiq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kavjueec.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dytekojo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fhkffcvb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttpqbwze.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2oeniffjd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2coeqfjqj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2shjjzayr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wljcryel.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2efjuyfnw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2veekesfm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ypckuypo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2buvhnwai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yzfgcwuy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ajjgmqpy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dlejzmgw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gbwpjohx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bvzvsrmu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mgnvsqyr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2avlmokyf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fylkrkti.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xbddibya.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2guzihzmt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uzmdptop.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrmlwfkb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kvxtypmv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ttrbsfop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cthjnzrd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2egyqsmzv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kpongmao.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2eqsqueup.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nguageqq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bjitmsnb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ujheucxb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fkuipelf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2uvsoeccx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2eucvemzb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2utzaoipx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jfldpnpq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pcwmpmrh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vjtlnhdo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fjsrdzry.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fzotlxey.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rulrhykr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nexqyeik.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2korqekjx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gojfylij.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yanrqqek.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuyoavys.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gvuvdkrw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xrqrhtjy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hgpeuxim.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2foaudtjt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2onqbrpfn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2saiqhbki.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lghnxsuv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qxzkgnmj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vfticwrz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2agqetmei.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbsuxxfs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2puqczguj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2knlpvmoj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2otqyatdt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iryyxare.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hotgbhzy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hpygroae.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tpzqents.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bzkkgyly.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xxapcuyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yrhvgcee.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2czpeajkd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uyszkumy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2algsmdgk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ccqgbrkz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rqsqkynf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tqrqbvyd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2prmvbyds.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kwdnrcrc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ioctcfxu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vaujdzxe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ctkezvba.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bbiifmbh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fzlwpxbh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ngyxayig.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cshnofcb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vnibxxjp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzmqwsyn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2skwpwnkf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bzshxtvg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2alqecpah.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2farhktbd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jjuzltly.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2onywfqxh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2inanyzmp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tjnaxnqc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iozjcaxl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qyjvfipy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oknhldjl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iisklxwg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hraimluo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dlqjxohu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2binqgocq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2spenegrk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwafpj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2axkzvhge.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ksejohin.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kwygpfni.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hmsgqdxk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fqqvtkwz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wrtsjrar.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bkjkdlgm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vslxnjdj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xwfobpqa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2agaqftrt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvqbbzdw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oewdkwdk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aadmpdjx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hdmrtcgo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hfblkalc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zowlmunl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rpskzeot.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jbbwidup.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mrkwpxzo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2futwsmld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvnqynoz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cldkzzsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iequjlkz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2covyldog.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cwmndhin.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ysfzdrwg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2geuirmku.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2htrrewvv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2otpdnoeh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uxsdfaqq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2narmkueo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xcyzpfwz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2izbsjaku.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfmgnbo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhtoawsh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tylixvaz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2irokckex.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jpdalubu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lzgavjrg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lxpguyqk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hiabjaof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hqdziroj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ntixlgzl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bawmilmr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ngaujtwg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ueeavebb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zerjpabj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uyfcxcef.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hzmmzvkw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2guaamikr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bmvbzcrz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fbnnioxn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oziulhvd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zxfrvvin.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cgrfxiqk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vgkiyjxf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dwbxokya.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ttqkoekg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqtxqapk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdmoao.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vmcigyvy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gitjnnjz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nzzxtxou.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qhndselg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kqphplwf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xjiahmwj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iqzusnwm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bxgnxpqt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2siazuzop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2alkujezu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dpamlnlw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hrugiajc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cnvblmte.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nifhmrrp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ihvjksij.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2otkeqnig.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yxevuedf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vctzwbdo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hauafhlh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2blrcuwjc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hpxfilkx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hfamiuef.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzwzpbqr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yiijvvwq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eefapgdh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qzwhjexu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2smlrxuye.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dqgnljqx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2emlpttsw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aqbntvfs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wddpeuqq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2spnbzllt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2glngmqqm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wzasjmqh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2umhwrfbo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aunsfmgm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jnkprrra.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tdilrfth.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cfmwartt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wfwppkmz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aiyncqvi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2oeqbrynk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jbhapzjl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ecgnqyci.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cjeglmya.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pckgsmal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ckuehhpo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vqezwxyk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qeknphub.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbbndrbb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mjayxvvl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbqpgscg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pfagzuvw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cufyuyeu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nqzvwihk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rowcotrq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wxnscrqz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bdfleozd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2phopxbvq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mokdwpgt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2eoniflyz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibexldnt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ftfyezon.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cwbcwbju.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jnmhchis.html


<!-- 参考信息 -->