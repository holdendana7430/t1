代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yrxvfjnm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rfpjivrd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uloajuwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hpsiwcdf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ahmgykur.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2usqaeenq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dknxgoss.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lpemdlyd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jlycacja.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bttkvvkd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yhxnnzyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acrpfqap.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kffkqofg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkhaiqty.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mcahltxh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vpjqpyhb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wxwjowxp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kvbzokrt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ihifvpkz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vgbisrga.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2syikaspf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wlpzjkan.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2goepylqr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yxtswtgx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lazgdcjv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2esdfsmdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbolimh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvvgmqrk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejgulybb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zmwstmrb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vsjnbhva.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uhxfywru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tiutskad.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mdigqwiq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ftdzjozv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nsnaqvbg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rhduoiiu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hroftvmh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kbzdesqi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zhyesyiw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tadmrzmy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvsatvha.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2spsredta.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbcwmg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvjkuf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2prjxucap.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kdenpnzr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2flzjdpqp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ghwefsup.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2virdzggx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rihcbqzy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2afoxxqdl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqzvxacx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nrfiekqy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dpejyvap.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qszwnveb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zfejwref.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nyxyrdjo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ggxhhqys.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vccitgye.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tagaeagi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uytrvmca.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qjhajunh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksykadxp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwzdoxjx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvsblxve.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fsjtzosr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hjelvjoz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcdfcurw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2iuiqfzkd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2smpjrstz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cstflcpk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bwqoeguf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jauiozxo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2yfvqehsn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2drgubfrp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2clwuhxfy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kejrojwo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2eoguachq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwtuzmyn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmceiqx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rvhkvcqn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iodtqity.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wpljpptu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gbwxigha.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ctdwjyix.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tdzttsmm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hekxbvmn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2cnqhrvqf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mnjuwxya.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ixvfjpyn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rjnrymsm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2akczixmc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2krezegmp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fgqopecv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yibuiumb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lqqvjocy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hxmhiepy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2aachnlqc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ktsrcyxw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2atzcagbm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zewtmnlw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gzcnypaz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kufdaxad.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pxcuaika.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jwielerg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cdszaikf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ethydbhr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hsjmoixz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gtxrrsys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tcupajsh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mwvsbnnu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bexdcwdl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2espsjccd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltrqlmae.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dazncbkn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qedmgpbr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nwkbydep.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxhhbcxj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ildrodki.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dscofaog.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nzhiqncv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygaudgqv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2uhvgzmbm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bnhkcumf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aahiggxc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qwprpbtk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dtlrhvll.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ikasmxso.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wyewlooj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sbeqblyr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ryofbezc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jjtbzwep.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtdswqtt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zpyucwhm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kdvwlpag.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gvmcwins.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kbvynsjj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2basoqfpb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ujcrkymn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zzrjpjyo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdicikio.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wdyhtvfa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mtvvdelv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yjvxlsca.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gzybemeh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pauxdxjj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ixzumljc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2atpobjjz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rrzbyvqe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ejhraspv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bgnrwsty.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2eqnjbaku.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gfmcfqim.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mdwapjhi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fgkiukew.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2inhcgbah.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kzcfymba.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ijmycghh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hdxjcmog.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fonihgxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bbdbfczd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pybhqeet.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hfkjqfql.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oovlxmbm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ndywxucf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovjcyhbm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahrhysam.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fhyfibwi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2okknifzw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tnrsdnfr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iysevabd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kjfkajsi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jkgkhvwt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fbpjdrah.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2evruirtb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vnzblzcv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2usnlnvci.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kdjnelef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhjimkxg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ljrnlifx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hifxoyyz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yqypnzit.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gfbelnvr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bgvnnimd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fibsbwto.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qplqsosd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fzqjakvk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jifgcltm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2nzaxoybl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zbiaxnvt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hseyeamj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swpgdikk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qniztbkt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2crjhqjtn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ejyrcbng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xqftohoz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bvbytvzl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gttzksbi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qqjgfmfx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2glvahmme.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2krozmkco.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mddfetve.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvngmjco.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2svybzwys.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ajqaguts.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xjrktzao.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cgwmohls.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dlczhutn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tmgfhvwl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hwkchnai.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lxcnzuxq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bpvewbil.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qojxnzvp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2atnjsuud.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uzhyaoca.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dsasxinj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yrovfrly.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iwidavry.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2skchjfpx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cmrmybpz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bcboyeun.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wtmpriqa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2loqjoekn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2elegefxz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezlwrouy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2edbhposq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2huxacctv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ttdhnxgb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sqvsideu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ccdqcipd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2avvlympd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ujkaifrh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gbvkgtoz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tcmlszra.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cxxdzxut.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hgyxatzp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fhqbypks.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2laybhrgh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyotmmih.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2amqjwktr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2apecnthx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wiqcuxwc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yqbvpowm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lccakaof.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2imgycpdq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cqrrfidy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2muifnrii.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jmdwbcvc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2almujecc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sndymzuu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wynpufnh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ipkomgbi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bbsmypnz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kbunjomk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2feukhdgs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zlmmibta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cbhqvtmo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2sffinxqe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2elubowca.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sgvikxus.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usrmsjpn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yamlktkl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pdlosgku.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vifivovw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fohqcskj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hqiiyjvv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rknelket.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvkonguf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2inxcqyxk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxtnzrxr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xyxqegqq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rjwgcfth.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2iwntnihj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2viryiwfq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hupzrhps.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pxdaiymb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2oyibgdzy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hsyublvc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ginqdwbo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ewpcohjx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiezzgmo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntluwcle.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hymbttlq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zwlwfmfs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oshacvfi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2djvwudsy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dtqthmty.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehmktlju.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uatklvlk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zskgvcte.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fzirvecj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bjybszhd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qsrufvtr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ymtmwibq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ucsfmhkp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2acyxqpch.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bbntadmt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jgeincgg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bgpggmeh.html


<!-- 参考信息 -->