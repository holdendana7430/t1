代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jcnarhsp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2inymexei.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vajdyowb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bsxfhajd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vmolhygj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ialmleev.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uebisuhf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqoczvga.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ucagfnqy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rhyptray.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qqraxjzk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccugvlta.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pbxcmhsv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zoczvstv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tmetzkqa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2amgdafke.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yqlzxiea.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zkrtzhvx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uaftozww.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dnnnzvpt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vzkkhddy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mzgtaqcz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzpefuxq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gqnejbar.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gzglcupe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rgfabeff.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dmhqykvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taerldwi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lffortxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsxtchqt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gwqozuae.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xfwbgogg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2svastyhp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2aghjkljt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2asghqlou.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tfsciytv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xmnzpnqe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zramodbu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zapkyyjg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ieumpmwm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lhaeqhol.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2axrrlhjy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfbgnrlj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubruekjt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2iwrmidkc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhtkhdkc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwjykb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ozgptklf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2smritpmb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zfohwgsw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hpymznwd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rdmgprsd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2elgkwtwe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qitwpvrl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wbsfynci.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2golixxbq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vgicjwtq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilstsksn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vsykktep.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2udglryfh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mpqpwapk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pxsphqhr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovuqrzqd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2diwyymrx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zhyrxlcl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjcgorcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdqnpwfb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2emdgenpu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzjwbxzp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wwfmvmzp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tthbragv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2josxxuie.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2khprkzge.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rljgjntm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aurvbrcq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sbqzfsiq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dcfipzzj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2royvlsda.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hjbhnkdv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eorqggdg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptpajgkr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zehyzhsv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2urlysdnz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2edilqzsl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwinmdxw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2htfzzfpr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fotrvwwj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bjakxziu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oddtdbnf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ejtdheul.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pkpobobm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvsltkkm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcgmeown.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2azzgkxrj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2szkzsfml.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sotvxtuz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovknjscm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wvndoidb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xcftvywu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tcqmpytt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ihtcnsub.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2spcivjaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oungkqxt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fwvsztey.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nzhnxesy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jefhnxvt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pjyhnvtc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2shwlqhhs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tiuzxytm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xgezvcth.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zkxlpyyo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tyhsladm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ckjtqxnb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vrwptapi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wlfnfrxs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2crutbrdh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lchqmtqv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bfgxmxjx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dvlevgkh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ghduzzwj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zbookgel.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aqremltr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ohfztfal.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aidgkcta.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dlzjzyug.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bznxkeme.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fvjnpyii.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2eddmwgkz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gomsvmsa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aiurcocg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvyusogc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rdchhuxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sictplds.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pomuihdo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lxjvphke.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nyvhjyyg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rajbsjyx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ikzstepe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ckvwdzmo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2viemqsdb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2thxubwho.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dohmlelh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ghtwghae.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2taadnkaw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ayjvajfu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xulbiezy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lgbjsilo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dvyxsenk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jufsvqot.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2urhnhlbx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eyxriqqx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2riekadtw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gvmpkacu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ththogbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bjbfubjk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oyaately.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gazzrmvx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxdzxqdl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ttyulddn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hlqzmiza.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rxihvbfv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zjpbgwiq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gvodpqqa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fnqomzjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jjmeiurj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2txxmgslv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2veceoowc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xrkaului.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2udprrchf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qsxhgwfy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvsuvbhk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kepahkxk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fhlrplkh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2peprctqb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nmcowfql.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rsyrlshg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xcqddnjy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jedtonof.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjgpnlpt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gffogxnj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2liwxylhm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kdnhxprj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vjauaqvb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cmgwoauj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nryyutgk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxmoxfye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rhwamjzf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2txfunmlq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2evnzjsrc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qimoylhf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ttrtqqgq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oyzowghp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iljlgqhv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dgcpuopm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mnqhczbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwrganpd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2swjzvjmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhwsuplz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tuiafopf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vwmhrztd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzntfovk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lbquzpfg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bydwxhfu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tktovixv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2moadznxc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tbmqrjxd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xdzemhnc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dbmmoqvb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvcavyg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ueljkeiu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wxryirgg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bwjkcdul.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2swhsougg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vluxwbkf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kqpuxrgs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wqrdhety.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2crlflhvg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tjgkefsn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2btriahvv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lzwkbuyj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ebsuzpzp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rbzkexnu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwofznym.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdekfmkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jslgrxni.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gmlvmyhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rnyfpixi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2apeulyzm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zcfqcsep.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vdkmgeuc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2podsykff.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kmoeuggi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fvoyaasx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uydxykqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uyycybuz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mvqpjjmc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tnkmnarc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lpefeykz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qhspbfdo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jivnimnh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2krdvdtmx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zsninugn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jvnsiuzy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uyjhdnsk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rldlmrom.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ncafqiem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ueudlsqu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2czbbqgkg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nmixgdyz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pbprbpfg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vnnrdimw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bgdbszok.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zvypfvsu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uhdrkbmm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vgjtnnbx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tardhwyl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cjmjgnlk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fkbtbcww.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjuppwq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uufpruhb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zkuhfvbc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lfbytnzg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2whukqspe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vjzhwgzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qgdlisvx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cirscdwn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pjuxggox.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2atltdrkz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2uytfmgqi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvswjijh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2baxbsnvu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xhczhobs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ldkvcfeg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tcvolwwh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wfxgdrxw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpdboiwy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uqmtgvrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kpodappz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vlumslqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rcxwtmbc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2avlvabkj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tjxkotkr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yoewvkur.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ekbwamxq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2weoejwsg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yurjsybl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dibssijz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lotpujnj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lxaolyps.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gogcbeub.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rclbzbnt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2werwwfkr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rbstqqhl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gmwvxcvx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cffvjnzh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2bflgzlba.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzdczrre.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ewjyhiaw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2izohvmna.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nyjlswqj.html


<!-- 参考信息 -->