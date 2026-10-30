代发 wailian999

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gzsuswwqx.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gnvorntnp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gypqqbfmc.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gkfedmgnd.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvhduebzw.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/giixshhlc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gnnvrnvxd.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gotudvocv.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gbjhuzjob.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/goejhvjfy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gpnmzdupm.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gkrhaykwp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gfxhquakr.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/goxgkdeyg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/goqgizpbp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gaaemznpk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gmnkgextq.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gqqtpzxfa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gzmlovhrk.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gdsuxnptw.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gwulhbiye.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gokcvzpjs.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gexhjacng.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gmsgnqlvh.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gyhxabqsx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gzijthblr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gvzrljuot.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/ghdortrps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gimtpjjvb.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/geeyuqhwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqlzwfzsn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gctfvtknp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/ganmfurdm.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gnqnledpf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gefgranja.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gxhhhlobc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gdukzdolu.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gfsdfmuhx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gmnmgsadw.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gsokurets.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/grcdpyfdf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/garszjark.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/grkfuudmp.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnirqyfhd.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gnhuoowuv.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gaberwylq.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gmdjyudfp.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gojdulcec.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gcwirbbpp.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gmhefrxqw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gfsckcwvr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/ggriidnkn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gydkyerxb.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gvkksrlnt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdehmpy.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gasssysvk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gbafjqznm.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gdndkwhjm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gpgxcltvj.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gbckhlnzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ggjtoxbpn.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gbzwndxfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gnjuttumc.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gkmgtrsaz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/glsfiwyfw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/glgdzlgtd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gnesgkklm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gwyrvitgb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gsnjnsvzp.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gnomryztf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gnqgpjdvl.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gwpwafkrp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gswrzutop.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gcnkwkesc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gvvytmdmh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gdopubmrt.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gzcbkkgag.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gmuqlcskn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gtbzmnmby.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gntpcmlqt.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/glnzsponn.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gqgpebpmi.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gbddkarpq.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gyfzhgfur.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gwuqcpsse.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gygdneddg.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gqssugbxa.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gftfkpxhv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gjiqeptow.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gjsnhoxfy.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gymtpwizp.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gsjvcbmzs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gxpckbkek.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gdivniuvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gypfhvkzi.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/grnszkmmt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghgbixzzq.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gfzhlfbur.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxaxdhkmn.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/ggvpejsey.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gofvoqulr.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gnrxksqar.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gfkruycof.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gqsiyoskn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gcfwatpoh.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gegylhlwh.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gmyhryoih.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gjdbedrbh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghhzigavv.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gfrknpqwh.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gztktplmt.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gskgxdail.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gpwqmfhrd.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gdwlthtoj.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gefdkifkh.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gmsrfijun.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gzeaejgrb.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gfvbhahrf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gqcpnrwaj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gmseqtjyl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gbihvjmap.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gikwavwcl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/ghrdviphs.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gcvjxmnsr.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gelbijnkh.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gjzniokuu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gpzalmrdm.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gufcvqgef.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gwgagcxmk.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwmbjkbia.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gydmhgklo.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gqpamzzhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gymubsmkj.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gzqgbqvxe.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gqfbydkco.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gjucgfiox.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gjrizpvto.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gznkcfnyv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gxweobcke.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ggmegjgag.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gliccyqer.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gyrjqzjjh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/guzbynfqp.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gyetvmgnv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gqydvtpgc.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/grjdhismv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gbxshlrlk.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/guabhtmjt.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gywnkbiqb.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gcfdektwk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/ghoycfale.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gjtfrletp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gtmhzgilp.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/guoaahcys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gplqzymzw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gapslqntd.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gcuxhhyyt.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gonycaovz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gbcbatpir.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/giaguifot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gyjddeljz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gzmozkknl.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gvpzxjwhd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfworkic.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ghpbezkbb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggnuluvpn.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbxusfvzk.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gfxqfcepp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gidhpxiby.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/guupcngsj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gpnzomvuv.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gbfifswxz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gxdmqvhxq.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gpfofnajy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gqwdjefzq.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gtyjvmeen.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gekpqvajw.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gndmduxlr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjbrgso.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gccothwas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gfzhkgdth.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gcbgxqhxv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gaputtxqi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gwyjpofmy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ggacunbrg.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gfootupgx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gufpbdaxs.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gsrbzceap.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gztunsjfm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gusuovqlm.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvmbilwso.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gdtclodms.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzfdlypkw.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gutcspmui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gtmjnqnng.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/grytzukqu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gfoelqlhc.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gnoibdcen.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/griqioefb.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gvuugxgya.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gtwphehai.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gutdcevry.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gjlrpunxl.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gyhnpderj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gzutlvpcs.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gerikiyfv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gtlktabin.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gmpkyxgqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtprexhrv.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gbtsjqbno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/glhnwoqwp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ggdyouwiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gffeqkgrq.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/glbjocuvx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gabgeadxa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gfvulyywc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gqqwjtsox.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ghschskvm.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gkitqekne.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/galemhpts.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gjydksydu.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gowtgovsy.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbobxlrll.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/ggbhhuizf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gjbxziyyd.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gbpdjestj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ggcusvkws.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gwqnwllme.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gifuyivew.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gqvewjybn.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ghudjbavw.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gpiicfnqc.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/ggsykhjwd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxamhbekn.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gbxmvkowu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gjkutxmnp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gpdnneswz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gjrcqjbip.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/grrkocsxi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ghfgbhtvr.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvteuizuz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpsroteuk.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/grmqfqfeh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gapwexvac.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gdwzmlghi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcgnksbrc.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gdtytzbqc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gwyoqeztw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gozqqloby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gatfrjcem.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gsrvfhigw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gnyfpjogl.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/grtjmqvro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gsxrsibut.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/grnbucomf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/grcvknxtw.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfuhtfvdm.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gmgjqavri.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gnbfbxyfa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/giozrqmek.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghdvqoajh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/givlenmur.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gmbwjixpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/ghhuzofmo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/giprgogjt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfdqgppr.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjnxjuorl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gcjpzdske.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gssjinuop.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gavipcamb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ganwlmsyq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gafjxdjst.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gybcrgxvl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gfnmzzbdr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gafwbtvbh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gadccedmi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwxerujs.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gfutohlcp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/glnudihjz.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gfsxlfnex.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gbwoxjsxi.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gpkstdjdg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/grjmhrzoc.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqydmxs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gtuoysrao.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gtkrhwkck.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/giywcupgu.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gincdiyep.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfxojxzxl.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gdrjrwchw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gsiiwewco.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/guunofkjg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvsuooyuc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnmvudlym.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gvizmsbbl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glpfvbinf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyspxsfho.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmlvcswyc.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gyqopfpcl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/grriarthf.sHtML


<!-- 参考信息 -->