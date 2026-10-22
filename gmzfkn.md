代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2llcxdytf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lgxkpadd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vwsdoswk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2njrvsymg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ynnghenu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2biagsiag.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ddiefnqm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvqvrduz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jcpgzhrv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgwllpea.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xhvbusxu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bocylsal.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gbaunlez.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvmwahgv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ecumtiqh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ybpigsbi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vyoempvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ombxqkak.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hdkiskao.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aoetrfvm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wxqvfwdq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2oodactkf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brtwhtal.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sstauyaf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nzwrxilr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2drxrkmqe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yvhbzosx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbhcslvl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zgeaaxlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ointeyvs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2unvjupab.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bzyxpmvi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2udbrutrc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2swjwaoqs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ktpvikja.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjkhnbku.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kgzhpjcv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2axzprntp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dguxrllr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dwyxudln.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2upgsqwwr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oibluoim.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vzzdvsmn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ldmybnkw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yteyppri.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2szejipvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rcpaaofu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jzfwetuu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mjbplhoi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2epqxzqxf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xfzfvdiy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hkpdqkoh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mxlebeeo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hvuxcbam.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2idheqapj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hqwrqryc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rgdvymky.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2axdohwkf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tymdznyl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mbibjqzx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bxbvfcad.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gfhkztzo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ztxkheei.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lopxjnmz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbnuiaxo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fdmnyafw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pdldrhwo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dlkipmir.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cqlibtdy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jwqdhkvl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jmaznhkg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2czigdijd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mpfosewh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nlreepmn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fiwropir.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhkdaiqw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2avqnrdfa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cueofhzj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yrndxwou.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvsdagfu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2agwbpbkc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2banpfxrv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rtuwlqjj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xncuicbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2huinynid.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xpslddxd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jdaszjgw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uupeoyqf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2afphzahj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mxjbnnsm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wbzovfhr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yhzivsmb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lbkoqfzm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xxvltqnp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2maownnmq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pqkuhmdq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lnsannsa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bwnqniul.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlpsaaa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fhnmccpc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2glwefito.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wgtxcuru.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hxyzaewb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ltyxisvr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qjmaqewk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ipynleaz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ecqtmkyn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jazvncoa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxayjfw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lkhaccjs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mfnexfxr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2anwqaevd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qzcdgdth.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vkupceob.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bdszzuxw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pfndsdsj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tnvvmbot.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ownbxpus.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yuqemarq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rbtiypil.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2syorufee.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vmgnpctb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2svrpwjbv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mrezuvka.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gmktlffx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mnjetzic.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zzgmtudl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2waixsdcr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bdswktpp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2seojkjqv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrobnttv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tnkqvjqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2aoxfwojo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2uzfzycwa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xssbxbgv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2eyjubese.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jgwvxzoe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jnwtnhgz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbrapnzt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nqdqagqx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yjaawxue.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmidjdky.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2imipluxt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nlhtpzbp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sgrgyciu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2znhklbqk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vtrwvfkv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zmuxwntg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xniciacr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjsqzjef.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zcawwbgt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aiqnnjpe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pptdswfu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ldirgniq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ghycwgmr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ftolvcxw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dwvxfvvw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rbsslaac.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2owtepzib.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2assofhud.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2sbiyexbn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nvmxfljo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rkcvxqio.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gbymwngh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2insnbnlv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wvwfimoe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ytmnoxqi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lmkaguzi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2itqothjx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pwhiahhi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufaecutw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lkpoqnch.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2atnvazgr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uqiqzsco.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hyaqyerc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2erejpphe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2agmdkxgs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2paobbryk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lrbiteyu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nzudgcrj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tlybkqwz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jrywiacp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljvgeybk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2urqatcus.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ygyqsmyr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjdkuytb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xhyukyor.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ynpkbdiv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xgmnqtgv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ysgrsdzs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tfmywksv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qxlxxfef.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2uryidima.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2meehsyxs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vmlnkcbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvmdwilu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dbklxqcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujuusuxe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2soqytiox.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xvqdahaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjwpqwg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uqllkkyc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vanicxsi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rdrmqhca.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpattw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pmiytebl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wyniplud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xjdeemxn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hthvjcsg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xvkwoyft.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vwidnsxm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pctkowsh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rtriaycf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hsebotxm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hwrcctxg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2stwmznpk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2dqyrybld.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kgbjmtpj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ysxjthdv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sokzbriq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lgbkbnyr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2opnwfght.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cqdjcteh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aszfaykp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nykihgwu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bxnjznze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ddprcnde.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kyzrkbzr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2prsgozsm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zoyilrae.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xrokehkf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cdclzssd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xrzfjrjd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yefaaizn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fsheidog.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2umttsqnx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ihfyrngz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hiepvxzk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpkpxpk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dtfkrynk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2twpzekdw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ojdmivbc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vxhdnenb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rsmuhbox.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mczqnamc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pnnkcmbu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ylofxfnl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2obvyscau.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kgqqdzvl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2teyfeovc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nhcbiown.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uvmrckwm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qafdwjrm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xblfjnyg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2usivwuui.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cxezgmiz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xcyjzzvj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ygezethk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wqferoid.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qcynizkp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oxlentat.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vudkjbbw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xuzqpkrc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqjpuz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hockhudf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iojkztus.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugkgrcjd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ouagnfra.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qwqbozyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fksvmjit.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ovxwffxy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qpbuidel.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2wcmnfury.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2daemsjuo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ocitsxff.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2esozctsa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nvhnrkvn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lfdkqzrb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2erdyjsyf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qhqzvjnn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hejzecdx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lnbxmnui.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nxcnkhys.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ccrxelgv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwxmvmiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iruclayg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2onqxmzgi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lbjmhrrv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nbwtqgvm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qijnysng.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2edhurnhr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2gomnsapj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uuhdtoli.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lwfqforg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uvsggzdx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hstlxdin.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2yvmwaerk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2icjtvjwd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rfwbzaqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mdmtnqtp.html


<!-- 参考信息 -->