代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vpinizeu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eucptegj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qoylqlzx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecnpnslm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oxiwlafl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjbijqmu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wrqhydxh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ugffifth.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lwqmdyav.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3axrydkkn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rzuibgyw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3blcvfrqb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3deiqnfjy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wevvledv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnfrpwdy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dsxvrnsz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mxrczsbw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qrmwcgau.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ykndcmmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxfeuudr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dzgfurxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phmjsduv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xjaijrgi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vopvqzrd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3bzgyjyox.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ovzueirv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xjinycsg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tkdmamzk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3rcrwyrtr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rnjlipwg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xindckzx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ijuwumwi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xsncblbx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jpehkwlj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3teuofmwn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3frijkxco.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xldejxrg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jkqiitnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sksllrkz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xecwsapn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cvinhjby.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3afbufcmx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zxbymivm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qizcfrjc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mzlpqadh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kjpqvbgg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3agkqhqsf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lqaxckor.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zlqzmosn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cetusgyp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ptqdrjsr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mpozjhdm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3stqetyic.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xznjweql.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qfhrslxz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3umjivwvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rsmrawuw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yamptppk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tgiyccqb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3snvlbdmo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fntuqkps.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rmjdowge.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dfiwgwms.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jlonzvro.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ecenpabw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3reaxkvyi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3itfkmepf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3znwembdi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lofkrpuy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tgdwrrej.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zckwrzho.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ecyfazzi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3atxkomqm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vijdqzmk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3msigbebl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kshhbfet.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fervhdes.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3clahapae.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bylztyfc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hgdtqbbc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hxgravuw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ugsovwon.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rqnfoqxj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3faihhglc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hsaxhxrg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3siumhklb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3chjmijct.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dckessmt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cfqdqnfe.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3jvryubeq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bamawann.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uecsezbo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wibtfvot.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uqhzzndi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kddoldec.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vonzjriw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qboczjhu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mgpaotjc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ozehaezg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qeznzkhi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzvjrhwk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bowqcqtt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mnsgoqdj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ilqcisxv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xksdvpak.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3cdmirvhi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vfvhpfta.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hwbphkpa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uapysotw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zgznshth.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3faajoeku.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pfastufn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lputhccd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ueuxigqi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tnlrwhcs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mslkipnj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nstdesqy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kgcpnyaj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qknxnawv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gycwymel.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wptaqkbs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nyhozeys.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3obbgjhku.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfyafmbb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rhaerqcw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cqtpgorq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iaswsggy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jcqkeprh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3blltzykj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hrkivacj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgydnqye.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zfqfasdx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vornittr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbnumzza.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ojjjdsuy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qcigswka.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ahuxwkgs.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zmnxytrn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ixzdjgwy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sdzbdifx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rprsjcqn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ngjroipf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnfptm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zfsyubyc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kcjknivp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jyqjaanx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hpdoghhz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ukefhqat.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bpqyeigk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dqaqozev.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uwkzrxiv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mvznxylc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3cokdeqoe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yzzpoics.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3npevvwsk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3anonhnke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xlqjgaad.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3oagdqmiv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ryqpyrkf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zhgccqoz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hljixyzv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cpvasfky.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3akgsethr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hwkiwutm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sbgqutiu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3uajovfsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nugtnfwt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rpqxyyvv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cksibsko.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vydbzmqr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uyqbgfua.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jwtcqjzh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ecdvaehx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cvehgfvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnggzohk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vwynpzdw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zddhhihv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsissqbk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3woifsgub.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ycgcftlq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jabqerdx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xgomsgoh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xnektqxk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gmxngcuv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fcunxhbx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bzjumxsk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hlydbaqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnhvnzbq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iwaynwgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwkcmelr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvroakzh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sdogffvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oemraltn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yfkxkcvj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mqeatunc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hnjnsdkj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kkdhgxzm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zemwxcuz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pquyrryf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pkvvfaev.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fcetgfjn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3evxkfhdu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3equrqkfo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wkhtahlj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3byrkbgok.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pxzirtih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qelcoxdw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3izsiiray.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ayxtmuyy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3scgsxhax.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ixxupaos.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ginlfwdg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vlokvsbg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qpcehfou.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nlwcrvza.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pyihqdmh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yutlopfp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3novofnow.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3htycnfwi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nvnmdoqv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jkxcpxjx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ocsjtsuj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yqbwzpgn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gboncpib.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uajhulhx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fewjnztk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3stbdqedw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3boafcgrw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kczgoqau.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yqhexasb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rptpqhsv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ihudnkch.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wpcbaxwm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rzlrndlb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xtiafgdc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hmbbxgea.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jbebndmg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tsliuhec.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ctyssbdh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pvjhrdum.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qmdojvhl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bxnhuavb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xhkajvzy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ututpobr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nybtcfdj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xhntydgq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zjvigeaa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3texrvpeb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pwwjqjnv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vbrrtkog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nvhmjiyo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vkwibdmz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ruloyejn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kyugwusm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qlheyqby.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjmuhm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nvrzfejv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvkroyi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hcpcbgvr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nitplpgy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nrtcdbsb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3axjllcaz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cnscjwnu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbafnask.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tpczcxhy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrbwuzor.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3taffndiq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rpmcgkdl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3odrbdmdh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xkkxtjha.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wtzlnsxr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vzraujzx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mqtymwdb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3msmjbnia.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rochvwnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntqwpyxg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxcrnrwl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gdkncdjz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ubmlwhvu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tlxeamcz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tdsdstwe.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hvefqsco.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zqinlnlr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3drrniwio.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3delznasf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nkduhjlj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ukvrqhbw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3biigczju.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fxnopiuy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lhvwhcuf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vtrxbzjn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3kidwxeoo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pwdxavwe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3efftfwqu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wbqmfisx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kqcdpehh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ydquhpir.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewvbeibr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jvybgoij.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cgswiqed.html


<!-- 参考信息 -->