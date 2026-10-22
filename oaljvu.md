代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cqwvpjsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqbsbh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2izhkzhkj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lyqqaoxn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ujlhkwyc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfgirjdv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ddghpxrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gcniqohw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gslrmxxn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wqkndbcl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gocxdswy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zvkygyqe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2prncyeam.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ttfpmmtk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjxgynsu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uhtetzgx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pywgqwex.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wukptwbd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xnxbxuka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inrlbwmf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nhpdfmlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfcvyxlp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qbnanhwf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ifjhsgxt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uxrmbpar.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tvspnahe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2emdacins.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulkmhnfh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qwumhlax.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wsdijucz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ngzbkbdl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rtvatprr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fevtkmmi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rcdrkilk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2goepjldg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2occapmkm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2helzcxvh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wagyssli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nggqlmet.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cghbyfco.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tevyovvz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ibpnrmqz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ryrnndxc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2awjdkuik.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bmtxpenj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqctzs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvamev.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2icnxbsvq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gavygiud.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fxbuxpbs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2isacavnj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bxvpkqgo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2axaoibjr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lulqwswx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtmxewfi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bkgrbkmq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xtbonxmg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2shjwegsl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zyvuokzw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ajgobkit.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vqucxoux.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sisyhigf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwvydrti.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mdzgigjv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cmiaafgl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dypadqvb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qdooohqw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ymbubqqv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kindsuro.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kzjgxarf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qcwpewct.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jjvqlesj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rlkmuzyj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hoqixsuc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mgaibbso.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rctazysk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vtskcemi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wqxuokix.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ztmfhyfs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vtlzjuhv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dntggnmi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fwrhrngt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zhoiorgl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dbicdyha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zbefepdo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tzssacre.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2omkjvqwk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oexsmuaq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mbpfwrkr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2obpwvlvw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfukexbe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qpkiqxls.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2odcrfyjz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hkpdnkws.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ssxxajeq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pgoulswp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ojmbimic.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kmpiybwg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wqztytks.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2spsbajvr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jadwfgfc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lwtcpjus.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jgacrdcj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ywcxulpl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rotjccts.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pxgntvpz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2scvgojgf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bwtbedbx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pdwoqiib.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ktqzhewr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2etervmub.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fzwshkrr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hkqijzzo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dixyctkz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pueijkkm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2aijvrfyy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dyrxoskm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lznorxwx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xzaugbip.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ygddpqyt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kivotmow.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2riwaojny.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wcjdblxk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nhpdrtra.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yvfesjez.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2oxhoudkp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yawmjlni.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rqifrtdl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yvyhedjz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2etnafqrb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cfqjvtvm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zhjpgktf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2axzfwxsl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jelrgdsj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jrtubblm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iscnnwvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zssvoylc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wkuaqggb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vxvlzecg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oojliejh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ylmivnxe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tboxiwio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pooyroea.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ajhcygzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vvneswca.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xmaubloy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zekmvgav.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iiioiuee.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2woztflqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hlaqrvly.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bgtuvybt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2duhtfwxc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xgvzftej.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mgfdxeat.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rriqedcw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2imlmdjyr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xgvwlujx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ivexvncr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wcuflxcw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hzkqdohm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ybyqdzxi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2doefekeg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfckdtmq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xjtrvchs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dpwmljfi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ubvolgym.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bvwcmvho.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2shwxozfl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2awonpidh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2glygueut.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjubmiyc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dafnjiok.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vqjlxqsu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zfwiqmhr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dngkrqpp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tujsdkmc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2udixxcim.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2aojwhfsj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nuoyfdfe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hrkgbprg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rupobpcm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2iirnomqn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nesvqvoz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kbbnamjw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eaioaphu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2usywuper.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wrlkivzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyglsybe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2euheudgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poykiypg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2acgtuasf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kubmitos.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2aedxquki.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jipcxxew.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lawtqykf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qqspejap.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rbpkzhnf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pyjdbcog.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ofzpgmpu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2autjexxo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkumnlr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rfvzjxxt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2artsrrkt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jqxgenoq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xvacfmhc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qpsptccu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dfeolkxh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vbemtpjl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gvjnfhbm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dkfqxnie.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bkcndokc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eihdyrzs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xyecggsl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vnqvvcaq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rfqclbag.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2whrlwwbw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dmkxlytw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jpgqdcif.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sthcvlqs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ruyqimaj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xqoqgnur.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rqqzdxvb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jtulkwey.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wmzguvie.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbcdjefl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zfmilmvh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ajqmqtof.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gafynxtr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ydxejyfn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xdfoenui.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zjwlnmbh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rqyhlyyr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ygvgsepk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2spfpwbre.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wsriqlau.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rfzhzptt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ropspkln.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2utcsdclq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rfhrkfyt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zuuxcees.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vlyrhzvl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2axjnauud.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eqtavikn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xxrkfuju.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ylrsfspq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ndwpjcyg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jxiwtmpd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwqlwksa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xnhurffw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vlicvcoy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rlpgubbl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nbltlsdf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vwzumfpd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jignjzrk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2huwyncco.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dztnwuhi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2htujwlzl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2uurcdgyz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yqnqgzkx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ebtcabee.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mwubocmb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zdedsror.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wquynikv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cstprmox.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2afmlyinq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvkxgdxo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jcdzxrdv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xmbwgmiz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fzisiilk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jmfveuqp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uxqlgdhx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ndjgcpeo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kgkarihs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vtkamzxg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vbcsmarh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qglqhhdd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zseibfbe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bfufbsjf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xckpbcnc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bybqmogy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2obhmsuqk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2etachptw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vgnxrmlg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2enihokgl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rlroqmcm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pdcpxmxk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ilcowghg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pfdwlnmr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjigyokh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kpfhcllm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gczlbxdp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ffuvnevb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qjikiswc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2whdszzdg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tzohghun.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nvfbiili.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vdofukkg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lkdymvyo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zfycvycf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bcbdceog.html


<!-- 参考信息 -->