代发 wailian999

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ghlhfqnte.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezgyidlq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyavgfadv.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqvehcqsl.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gnhirkvwp.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggufeioua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdicala.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gueqiidnm.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswkuxysq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvdogfxli.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggriakiwo.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnrnnodeh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmewxsre.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gadymwnon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaixyqii.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjqpsthq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumhdvkqp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdtibcn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gljlxbhpx.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gskocaznz.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gteafgcxp.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsagjpjfo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjstpooec.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/goxrzvszg.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/goplwbclf.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glvljxiyr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkmblnpn.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnweseyzo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggtfcwjbl.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzmmzfth.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbxlbdwf.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gykadhsbx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glpatimlw.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/giqmtuvvn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gduwycvcn.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxhycfos.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdxuveqb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtncmjig.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjkbibfz.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfwzravyq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxuygyer.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gjjwxqgkn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzwfijwu.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghoxryqrv.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmucgappw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqrqzazvp.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/goqwtrnsz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmezgrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyycymbs.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghywrarov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggioddjbw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/guyfjhuyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsokhtjvx.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gaxrtpcbp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzeoudq.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gccnzfcoe.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gijchucxk.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/ghylvkplu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gdhrtdibc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/guunqecoi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnkvlcodm.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndkpiij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/grtclitlt.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/grwujkqla.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhzuwjbp.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gkzpbqlhr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprfxwbmj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdulfrjbt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gnzypbewg.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafmrwkk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gavnkhqjn.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gejvxjpgp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdpvnuwm.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gacxhwmne.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqaafjx.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegejdsne.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcyzrgvi.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtdamujrx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghruvzdfh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gvubzuuri.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtusmsjcr.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/ggwzuhpvx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gjmneqtjf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfpbmwq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gimxajojb.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gzrzmssct.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjqfinsrl.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gabrzpchw.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/geawyxtzg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgmcmyn.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpgbpoa.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginryphrj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjcjgzqwh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohgwcwd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvoyzngw.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gntwbqmpd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmwgxvmfb.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gaayjzdzr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grickaqhx.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrhsdpsi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/guifnkdoh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmojmbiua.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ganlrxfbi.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gtcoxunuz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gcmzrisjf.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gteppsift.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geirbiftf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycjwrfi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsadhvbmy.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gufqneseo.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grrfwjafr.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ggwhaqggp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gffpocjrp.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glmyzifcg.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyburmba.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gslzfinzh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpflgyziv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxbrupkd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gziptnvlf.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gzhjocqez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfxesrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngxwrouc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gibhenolf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/glvlhdssr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufwymqa.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gofclavdc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gihcgpwpm.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gygawsusy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gsjdftwza.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmgbmxns.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gybpjoraz.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvaueagd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshsjype.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqrkxml.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemvqqkt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/glundwlez.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gyhwmqhec.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gsiqgxtgg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gldctffrx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczpespze.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ggxozsbmm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/grdterxla.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxmiinrr.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gragqrphg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gfccpjryw.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gqljgmfix.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxlxxkkk.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gccnzpksx.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gxajagkee.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/ganzqjyxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfcufxqm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyypevxtt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/grutbrggr.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldnlqzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynwkihs.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtngzbuzq.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gqtrosfmn.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtrcqtaa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkuyhwfb.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmdxbaeb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnbcygznb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghsaqnzop.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhyfvnif.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gryuibrmk.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gevnqyiov.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxlfutcw.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfvstcmvf.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gneyrkkxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/glwckawhs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoogeubk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpetybfun.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gwlradhhq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzokzkym.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gayivsers.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gitxzdyvi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtioyqlux.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlvborhb.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnqlywphm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktgtkhoh.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmrrjzbpv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gofcxuywo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwqsukeu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gavqcwsem.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gebdxqiwp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbjrmzgw.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgunkejq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsopmmhl.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ginbblgxb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gtjnkpmum.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvvdhpis.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glewyqmdu.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdiofiwbr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtqhynbc.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdaaxvba.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuugqhab.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzzreflr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gihlfzodo.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbdzbpae.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gatjnkkio.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxbzhxlx.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gysggufnl.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjwnsnuc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyamqxwe.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grxdlnufj.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/geydtftgx.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxdmgdpxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhfosyll.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gkabcnjpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnjqrpvns.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gzrmshnos.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gbpphfvla.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gylasliyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwijvxrp.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdegkwom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgkjtyav.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfltoxhh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzgfosak.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxoojtst.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/guemfwejv.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsfizfhm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxzcxqrgn.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtuauqqaj.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbhlzcej.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/goytadxhx.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gpoqbtwcz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafurwitv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmafmwxzt.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezeyvrw.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gdanvdgqn.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlrpxzxm.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gwyobmsrp.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcqimvnmv.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gspictjsl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzetxvyvx.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttlxoxu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeopqisc.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrmgizj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiydeapr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gkprxtsdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvmzqvmy.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gworjtics.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxeuhhnyu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gojrfldam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohuqsfoc.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/grobtxcij.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpitbokng.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuurqncz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaztgapob.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtfhyveo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/grtasjbsw.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gqedxpohx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgtyiaz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjyubjofw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/guelukjsy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbenbjjt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoeerstt.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gqquedyby.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqmhfom.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzflhhp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqhwhii.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkzwtrmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gleyubjio.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gdzacoepn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfsxqmcs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvnbzrsqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzlwrueo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxivoga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhrwntvz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpayexjyz.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaarvijs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgyrnhtg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdsbravp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzofwybga.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gersaives.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcxcnimm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzwvdpbd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjbptta.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/grettsstr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmhfswuu.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwiqkuew.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/graexhyan.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gunmndteq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbngsudw.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ghoerqnfb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkpnmaqza.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gctkpprnf.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gomiwddur.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixjvmlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgrhdphe.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzheyglei.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqslseckz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpefouugd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gaftwsmoq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geleufdih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxycsaopu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gacmggyiy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glhkbtodx.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/genjifyyy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguzebfcx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gkqdpkjve.sHtML


<!-- 参考信息 -->