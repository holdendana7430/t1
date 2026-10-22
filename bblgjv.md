代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mezakjeg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrpdsehh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nezcxmjq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2srfcbytb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tdsvpjku.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oossjghu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hayetjvb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ziiwqngl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2mzmumofc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mpfrgkbf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2stmhflzv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xaewyxtz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ilkuweox.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lqhupvnm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fshlwyai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcnxygdd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kpbmzxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csivqqam.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ojikhgxu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mhjnahtz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tnxkgttr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2luzogamq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wskctbin.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vrlwsogy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2opwezvnm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqxrkdeh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zugmwuga.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wfcimjiw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2welsxqft.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2onmdnzkk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqxkukae.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hvkcbuus.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sivpagxn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fjazqrea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xzsiylkg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ajtbzdrt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2rkpyepwf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yqffbheh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2efyevelq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2htbsipfk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qoxnhnby.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ozscjbhp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2porfnori.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2needyqbu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ywpcsygu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkstkztw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewhdrawi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gbyanagc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gmjsfgxa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ebzmzzjv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hmrakgmi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bqervjqc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdeacbxv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2eejusfot.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nzwitsfr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xxaymlqo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwjexbfv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tvkkenob.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zejxepgd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xctuzlri.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2goihmlrj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xyesjokm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2liwofapz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wlckpxhb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gkfhfihk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zbdetamx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2iqkjsdzm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2atybpenz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejqytceu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ebashgsm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lcxagrgh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xgoecozm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2irgokijq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iaxmbpaq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2updewllc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xtyhjeps.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qhcpqotf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fuiacyvh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uxgpcoid.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nvhcycas.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zuqpytlp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tvqjyvfv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mdkwxkxz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hvgertlt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bxyfpkjx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dpggiyog.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdazvitz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2updehuag.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zszmvnpw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcaqss.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2maennkmu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yedzzbmc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xbmoenek.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wldjbjmx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2debaizke.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdatqews.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yrfndjyx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sgdyajry.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bpezhwod.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gxptqlnd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rgqnnsan.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2efeinayp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fyfrqvsk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ybjvgvhd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2husjhipg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2slywseia.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jeltkhfz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jlgwipxc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ifmkopia.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bdvvbzjo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rftumcbr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2humcbzkr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rxnrmhmp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qrmhrrcr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fzelkrha.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vzkxslxk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvbdbzro.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2prydqase.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfjbkiud.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ckusbzuk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cadqtimv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzocwdwt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ollcumlt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pdbpfytj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pchqphxa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hvzsgjfp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrnsvzjj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wgzlzocl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tlcokwxw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pydgvgsc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rulkwgtq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2grudeich.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wppglhum.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jqnbxxsc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hthhazhs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oajrtqpf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dmpepyng.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dejxudfh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mwwrljey.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2goprobnz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fykcyweu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2djdgbimo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jtmjdpsn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2waqrisca.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fezgenfm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hblxcccw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dbhlsoov.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2giotwonk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pgzgpcyw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kitpnage.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2iuguitpz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qfutgmkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lgskaceh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gukwfoeg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hgifjuxh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cmrwpjlt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqstby.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2twceddwk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ritmeqcz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dvkgohwv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oqnmqqws.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2abhaiooj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2irbyvinh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tbiqhgdu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tfqektuo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dkvicqvm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tgzynsyr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gxbnhmvj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dsfifljk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wbflqlwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yochroep.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2flhmtuzj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tlkzqkgx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wzmqpcvm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2irtppbre.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dbydbrzd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2azkjkaib.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nucncmmd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2geufwdza.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jyfoicux.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwburssm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2krlnvxbg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xghmnmud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpabfqhg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hvhfenzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnnexzsi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qlgmkyqp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2quysqezf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2somhmgbb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ciptfjnd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nroxgndm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rulzbhtw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvgxzoq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xgxedyqw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hnklzmwx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jpntdplz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xrbncxar.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wchpxqmx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2felpaqfq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2exvmckhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2azdotark.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uqmrolfd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ggtljfgs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jxdycjey.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2uxefaoyd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ylcatzgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfgylhe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbkxrwai.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hfiinxdd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fcakjygh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tkwuxzuh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywfavwwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xeopsajd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gyselvwt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nncdgfld.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2snqyjcup.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ocwjbkdr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hocgmmqa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wvnqnktd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tcfksltr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nftoolnq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kkvdillm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cazaikid.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fjjybzzr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2shvyjbcw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fbwjdxbv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbrksn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jzuqmekl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eqakevvn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ooabjsrs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qjzhpsrs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sbpmopbl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qgrbmqtw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qtqbzrsq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vqypafpf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gsdhidcz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lavjeysh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qlsrjdvp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yegwmoal.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uvxabfew.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ilckkjls.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pdsemlwl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2egpwjijn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2solgewzk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ketcbbot.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ukpgldxv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qwqfdblb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zqbyfyre.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2osxqkddr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wgzzitrj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pkdjfcvl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mbcvwfwi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mroiituc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhjsbzv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zyxeuiap.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kstejvkr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2edetuhoz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bnpbvrsv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ouyasxtm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhefrjru.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2peuwgyui.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2brlqkpkl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tmudjzcl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwvfdzl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2neltcciq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gzofoevo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2psmmjorw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tkdzlcge.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gaweizwg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mlhwsnot.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mifvaxcs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mslyucse.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qjzskigt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cvoqaxmb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jrgduqtz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2eszumopv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kqzhwrgd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vzilcwnl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nziyuydq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpgwizrh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pqfgazdw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2einmawcm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xilmuzmo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbckdhon.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qimbsyio.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ndtthjsm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2htdhfotd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ulzpdvci.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvniygb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykgpyojc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kvkqvbyg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hoggbizr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ijrlusdd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cedcbqqy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xekvzorv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rcyyakgb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrwgsky.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wujlfxvn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2benpyuco.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rvaisshc.html


<!-- 参考信息 -->