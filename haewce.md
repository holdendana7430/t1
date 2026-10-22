代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vqhvxqbe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rtwkwxyu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gyhsgiew.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2plqlxtkc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qgzikjxc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rchfhabm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2atlqbwcu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iawegpgy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eucohntt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjflazns.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rwdecgtn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kpuqfodg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2otwmbpbt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmrhnenv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2efuddmji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vnnecqts.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qsdgecgf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2blcgvulk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2npkkczzm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gufnzckf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ininnaad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wpbdogum.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xrdalwyo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fpcdfqwk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kkrhhsqp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ioixcuki.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xhirbkas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iifxnimv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ugdqxzkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qapgkhaf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2whqmyvuf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2girtdvhx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oeqxtphc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zjbijuqw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jgnuwgdx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yrhofcsa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gdexygyk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccddbprm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vwbqzvwo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wqfsqpvr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xfckahnn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fvjwztok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wpeywjyu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nbfnglgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iwrnxifr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ncsntxid.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ghzuwwip.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwvvpynh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ijrqevfv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqxrqrjv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mzdevtua.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nsdyailj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yihqqpvr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yunlybuu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kwmizmpz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wxdgadbj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bvzmdafa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iypbafkb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qnprstgs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dmymtajf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ybldfdyw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dtwcafco.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2imluqufs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hhzhwbmj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nnovuwao.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2foawdiza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bxpayoiu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bbnyipgv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zwpqrgpu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rtxwnrak.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rdlrmzql.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2keojislf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2etmrrjsl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tialprwl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vxytllgh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jbhkwltq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqsvmsph.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2odvjwpoo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hkdmcbsb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tltnjsxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yoncvhmf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cyqxnvej.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ivuywdig.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2palacfvu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zubsndeg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dftipulq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uhhpktcc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mmjrtsgw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lguwteav.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mrdxvklk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2omjqzlit.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqqlwjmo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hvxvdxqb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dtxkhhjn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mhmmeaer.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2znohcqbz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2znzovapw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dumwbqst.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvftsadc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kkotcfhk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ceveiikx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2sgeadldh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2romrocgk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iavzkgtb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zuduufez.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2roswfkga.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ibnxwcxa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cxmbytnr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2txwsusem.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zngtroyc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cxnwmpkr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xsejjtdt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pubthpht.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kgymwekx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ugycekqo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2duyzffye.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qxycnxcu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uwnihrvv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crnoapgy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ksorfnii.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2elqdkdcj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jzthskhq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yqbcftwj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rextztjv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jejixbew.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wiuqhmny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hrhsohpn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jzzjlyal.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zeeikqrk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qdanevaf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xmneqymm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tsqgwhjm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2naxjilsa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hiistsuk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eikhjnji.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qzejdoab.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hlrgdrii.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qtmpssau.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ryclzxaj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dyqwkyks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kvorhrmr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hocohhul.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zcqfxnwx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gqpztrpw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yigahxxq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pystxkjp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ojxqxzun.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bylimrik.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zewusbuz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2erawnbgw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ssmjpqeh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tthihtqq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kjlgaguj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ukmtaweu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lvtibiqc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ipbajcnp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jbvzgext.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lpjyuuch.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ubuiukwv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xvwsbyla.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mcbxjsqh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ydtgmhjc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tvdybnvp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sloipygv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kwhvotpw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yqgulliw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2akofwpam.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ehkfbzhc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tfrvclsj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tjkotlbk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tirnmzov.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oljyujap.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yoiwhfvi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lxcmftwn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2simywvll.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2okyiyygn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lmpngluu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ovrvpxfy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qhgelkbo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ewgenjok.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xsvlogot.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zveaobbe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwnhhnpr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xglwlqmx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uguntcee.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ebgfytob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mfazwvtq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nkhorbpj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tldyptrl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pthbtafz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2usmepize.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pdnqapmq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmlwlqrd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qlqkfpun.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kfnszpxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czplopgg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rcnbgkdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhlneeks.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rhunjbvk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qdjkchrb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ktmqwmgh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2okenloab.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cuachbhj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2niiqqktl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mevcatbq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2knnqmvgy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yzbeaxuc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgqlalwi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jeejzmmb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lidnqnff.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fdslwzkl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tqteoduw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vpuhlokj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ragzpykp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2coatzumf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ukvixhod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bhlkldrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qwldmdjs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uhmsttfc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2soyukswc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hqzqvcwv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2smwijfwh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2feovcjoj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2shkkrizm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pcbsnqkf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lwfrrosh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2feewbjmz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pfcwgiby.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2btgycpmz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2koovczwz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vcxnwjbx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cbbarafx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oerekrwv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qilpbkwm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ffkjssan.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sqkfgdgt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hedezghh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zcxonvkn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2anmysewa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fqiacjdw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bbsltchv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bxajxqgj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jqbuczum.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dvmwcvoy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nlhvxmtu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kfmerwvu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lalrymkv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zkvngshb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2spijawsf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pgnektut.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2andigqec.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zaqyuoxv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ykrdxtyq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hagtdmmr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fuzdmgii.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvcmzlyk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dewylnxs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2sviheftg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aozwfery.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wgubhgsu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qzqrdlfz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ohtxunjn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gllqayta.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdzuzgcb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bnouirjv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvuffouk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjfxcozv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mvqlmkfy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uvsfques.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxmdnxt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2easguxyg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgaouzfe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2esuktgah.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2veghuqgy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ippqfell.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2guoemvoy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2idkhlvzs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nnqweczn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nbcosnec.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qksiftle.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pvcyvlir.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xamrvykw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jxrgtvxh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycdqabis.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nrvtzlwx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bgvyqjyr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfluyjws.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vvhbsbgp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tnibugtf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qyzeoimg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gxwpqlwu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cflnekdr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tbgtvhtv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrcixq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ukdkismr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amxnqxle.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrexnrcb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2thaqmrfo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mycegstv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nunffsnz.html


<!-- 参考信息 -->