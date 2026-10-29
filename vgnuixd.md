代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/ggdeumpzg.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gcronktee.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gikanyzol.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gweidlnbj.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gfiwqoknj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfsshprsr.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gywyzswno.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gyzpiaeyz.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gszzktdsk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gscipuyuz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gbubomeyi.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gqcluskwg.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gwovtpxzm.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/glvwzphfm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gbnskauzs.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gccrwpnuo.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gkihjympt.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/ggsfpltkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gliswqssj.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gdehbwfvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gqzkifjxu.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gcpzbexnz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gjdorfpco.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gladhlvva.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gavjrmpdq.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/groaxaiin.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gouzvyoqh.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ghswxopki.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gqbyidhgc.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gxmgomnij.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gubdrtzaf.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gznabhssy.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/guxuihfid.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/ggpmclzid.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gfvesbwwm.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gcpvkuntc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdlcoolwh.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gbsasmwxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gbrquabwc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvstkjlhm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gwaermjvn.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/ggfugbxwg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gifhfnenq.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gwtpeoycs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/getlpoiyx.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gdtyeibyz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/giyuhsvna.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/grtqkvrua.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gvrifgfoj.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/ghcbwsofg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gnsevvtjh.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gxncaiiat.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gqvbcxfac.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gcrwheyzw.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gdvvrznuy.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/ggesbowhj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gyfdgrtyt.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghkoxenog.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gvyexgkip.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gklejesly.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gkadykbzp.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gddlzejoy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gtgibmuan.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gkxlxgmum.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/glbjshlrz.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/giladjshr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gygtvipom.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gfjwecbov.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gosfjygkl.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxndpydsq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/galnrdabk.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gddcdvneh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/grseahdta.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gohoymonb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdonqlhti.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gkajzpofh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gzfmwjydl.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gwayiyyks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gofnqkklh.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gjlobttjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gwjctwgsp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gslwpgadm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gevehblqo.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gnorrhdyx.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gjlxhvpgl.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/glqvdphot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gkiewsbij.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gdoeskbcp.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/ghesttlli.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gabnxzrut.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/grrajpnth.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gefxulzem.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gqssqisin.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gzhtnqdpu.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gpekjyeuj.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gnbkwcpux.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gimqayftt.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/godxduluw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gcadngodf.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gubpmfghy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gduslccwx.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gtmcivrij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gjexkkfhn.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gyflclmyl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyvszxvre.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gaucykyxv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/goedhmlhk.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gfoawezxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gxplthwtv.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gytkzafro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/geifbpfeg.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gvhhhtfgv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gaeqwcmhx.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gjykyjpuq.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfngasqta.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gawlgjzyw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gbpxfnlkd.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/geebiihxr.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gbmmvvygv.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gcgnbbtaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/geymqdyxs.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gqhqlsquw.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gexhryhno.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/guoezszvq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gcidtcius.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/glboxjlzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gttyzsjps.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gknsouejw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gotvymwag.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gaxmskeca.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gezolrntp.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/glpzqsnte.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gzapearfl.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gcxqawjda.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gczhnruhj.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/ghxyemtec.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gsynsetfy.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gxvqiqtll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gjfehnfkn.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/ghkzjmexo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gjlwzkydu.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gdocvtvyf.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gbnrbykof.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gvhkjgiet.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/glffodrmz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gttoxikpm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gtqpqvhqw.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/goltgjgbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gzonbcbif.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/geyvfzevl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gbwvzgztr.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gjkctuzix.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gggclprsa.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/goyfyijff.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gzgcrxhjt.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/goyywowxp.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gnuwqiruu.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gjmcpmtiq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gjopdxchh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gsjjbwimq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gsfwkseer.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/glkyiriet.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/goaheadtw.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/ghwvkxaqx.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gejbwzxwq.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gxhbyrepv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/goyhsjpyh.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/goofjelol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/glrqgfvht.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/glakprsjj.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gatfbrqoa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guopsvvno.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/ghsggsizd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guciaicba.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gefmjrllj.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gmcbvzrgr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gnenbfebb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gmxidqlzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gutapndgb.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gksphtgqf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gztbywalv.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gcenbiqwv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmtmqfzmu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjdxnkixc.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gwunflrwm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gfcmwpmkv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/giscdytwb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/grdxutgyh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gxruikjhd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gokafkrvu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ggfyutrzb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gojqfqhkw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gqnywrrgn.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gfeleuvgb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gazmddvbl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gqwxlpvcn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gcabetvkr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/geekuykwc.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gutvpxafo.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/grxwhrhpi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gandnpuue.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gagojadoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gkifpylwe.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/goafoxebu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gcvbolwho.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggydaueog.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gdezpwteq.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gvjwlnbla.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpuskmqev.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gddwrdwsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gehfrmyhg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfxemrxgu.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkgsonsqu.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gprzmabod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gnuikxtnt.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gmpzwiukk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gstyqagpn.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ghzslgiso.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gyqkfpoyd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gzdnmdxkf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gnndsyjmw.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gkeeyhzec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gnbpfsctg.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gokdrctek.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/guzsmoubz.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gaziwnddc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/glodulzif.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gelivhboa.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gglpoxxof.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/goxybdlzq.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ggddwzgsy.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gnoyggyej.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gglqxeceb.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gfjcotpfs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gkudydfrd.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gnpwdesku.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvippbp.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/ghsttgpgj.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gmptnrcps.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtcgsmlxm.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gligrlzzf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gvwmgaqya.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gunmhaeom.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gufhoecnf.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gwxxgznpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/ghkxcxoby.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gizjialij.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gubahhnxw.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ggtelxaic.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjngyvplf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/ghhszeect.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtwzzpxol.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gcizpvgys.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/givyfmgzd.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gurjkyggw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gduewaoim.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gvlhmaoxc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/glmbpdtap.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gyyfrajxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gmeedbwrz.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/giuvafycl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/geuovujsg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gmvrmhkmm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gtfrxzafn.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/glutsmmtb.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/ghxhlqvws.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gufsymany.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gjqguhcrj.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gelzbtxmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gyvekqsxb.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gyyumdgxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gcctrncgs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ghscaxkxx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbttllare.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfjgbdzcc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gnrshwjhs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/grdddfdty.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gjpibmzom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ghegkdnlo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gdqpxrysz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbulvlawn.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gucdrsbqm.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gnkojptiu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gvzkxiqou.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gwojjykwe.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gifbfhtyk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gpifzuimx.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/grvrgzvrv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gwejljzbg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gsocbsmad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbkzqhhjh.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gcxgrzlcs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gkdlgsgrs.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gwckujdsc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/glubrabgp.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gbcbrgcuu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gyjbulkhh.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/glnzbehzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gzuoeetnf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gqiceyqlu.sHtML


<!-- 参考信息 -->