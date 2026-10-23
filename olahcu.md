代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bxtjdpdc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzlcfbif.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3catfatei.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ywolurgo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3glbfdkuy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wnqjubrt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kqbeazax.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3apmkrsot.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qqetplfr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hqbmvche.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmuntjzu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3shqcuobb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hrmxprqp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3exemjbhh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3znfvfhlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jroefsoz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ulwstyii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upcgbmps.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3escolfeb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pqjkfjoj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jarpfuby.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oqsegsxd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mfdocxbs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hiehyesi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qoehncuv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgwwzgbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hlfbhyje.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vfcwxjus.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hdchwqfs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qeaszjdi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ppetpfeq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bqambdof.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ajohxlkk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nxwapnil.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gkykndtw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ywdznygc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gdrfebmc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rsnvktel.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yzvzfqej.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mowqqxnf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qdzpkhhr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wwwdjtbp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aipdsskv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dylozqee.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bizgeoyu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqnrcqan.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zqfcttlm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zqddcahb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bdetgpts.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3imjeqalu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcunzosu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqtmucmg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pvkaozaj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dlzcyidb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ucpnwova.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pyyuziww.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hckzhclw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oumppepb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxedjtgb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3krwfplmn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbjyvvmj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3itwhtuvl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kyqgvgxi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgyhasee.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zrzvpomi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cikmmhjf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xclmnjkf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mcdsmghz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uvowdtka.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhlodmpz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uwmtsvav.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3znchgxlu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qkxoydux.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3bcolljzt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hnizfklm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ehksssav.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lqpmvqgp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3asoakwvl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3owmjgixv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wylwrfec.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fjvuhjqe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fsbtbazf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3iwicfsib.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ufkmhzuq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxeszgzw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hdymtsfs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mtpxbrlh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ytsmvhrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3joqmbbil.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ggjjuwgs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hynxxgpp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xcduygjx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3exwaeade.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xnpyaucg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3llvmoqxr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jwpmhmfj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3scqrpcil.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zghrzcuc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3obenljcf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wbwrkwaw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bxgpupiu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vqakgtbf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kstbbhyn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pbosarcf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3twbejsvk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ttvcqjvs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdwwwdtf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3usfzzppm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3blqnpegk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3arhmojlu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wbaczisn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nmoffbjx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sowqejkj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3llfnibft.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3awrfyeti.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ffgrcjgz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yuglmtjf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jacjbyun.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ygmthndp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3oityaode.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yemhzxxv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sqjtensv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ottjvkev.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ccwpdtuj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fflnjgcm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bxnstivw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hpztzhsf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mvigbvfm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dudtpbxo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvgudzed.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mrzslnbj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3waecsalg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3imxcyywc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3blrjzoqm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ogaschis.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nlcyazjq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pepleits.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qieypdvd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3iqekrhph.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pseoniuv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3txbjtdor.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xxfzkdia.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lgckzmnt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ivmdatyh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wgncsnsz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jayaplkx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vejkkutk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3iukmeird.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hkcideas.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cijxjhzu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gpamnjbt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bdysxgmh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3doxuycph.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pisbpqrf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dpohdnhj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lsadrkcv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nuryfufb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qbvzoohg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dnnwzacn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dmsvcqev.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fevkmocw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3htbydfoj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3viplylgc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pseuokxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3auewnvbl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yknjugte.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jfatogto.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3irpztbos.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3juhvpfba.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ctontqys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vfyywgyf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hkshxgvg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dlgzgffo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgfktzbb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fsaodgog.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bmqtwzhh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fgissupq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3umvuwbgu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tmbucfnm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ieyalweh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wildyzna.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3thzewtbu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ikrhzxpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfhiguya.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hyqmyhld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woginjhz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwauvpti.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nuzkgvha.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzvfgjoh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nmbrngqn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uklhdjvd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kzirwvjm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kpvusycg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ppbstudi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3guamyrge.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tfenydkx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cwuvgwbb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mvfmjpjh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uoscodkq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uspwebui.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mrxnhxgb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ssbirkzm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3pmkfzdyo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yevvysjl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gwymamty.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qmlgaxty.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3moohyyqd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3billosoq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3aquzzwmu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iexsxeii.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ojsacesa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vxvjnfwx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mzwaabqa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ecvbitvi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zhtfepsc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fbiwomif.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vdhklsam.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mrrzthmx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3inpcfepx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zdnbzavp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3biglbwuk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rknxcxax.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ckewjpqa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyddzi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qnttmnau.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3beypmivq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wjpogybp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mcpdwccb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ppakzubv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gsijfuoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sroktyjf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pbenpfmp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wsrhvkil.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mjvikuyn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pwdtldyj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rfefbska.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gceezuwk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxhevgrd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nikvrwwl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jddohkif.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iihymqdz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vgmolluf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aiciuqpo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3iltgwnvw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3usggimxi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fzrjzkty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rexfwind.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ildranmg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3noobvwjb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vhkubrpp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qlbwfqze.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mgtpwfqq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jvcgjtfk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3swpkcvkv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ufgkjzev.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ibielduc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tefqduue.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qihcmkmo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bnwloncn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3auqlpvii.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vthfbzes.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3huizpyhz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vywowjuq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lpyxenkw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3doujmovo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qkwdawfm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zipxmaxt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ofxxoase.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zqxbaixz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jftlrrim.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3syqmthfs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrqotgtq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jhnimlim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qvqinaxu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hlzjvsfe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nusfpman.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ggnutlng.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfnelm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tptyxcaj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3erahdlos.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qkrfkefl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wpolacyz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3edkudvby.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zowzuwvq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iyrfqtvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3govdphqa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrceegpn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rzlfgcyz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vuvypwhj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjfcxgca.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mucursha.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fxohdgwa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nahginlq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nzdzemai.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pvxzftep.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dkimcrtd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3khvxxqjq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xdzehxup.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3axukdruy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zzvhhnlj.html


<!-- 参考信息 -->