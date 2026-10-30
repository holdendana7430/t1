代发 wailian999

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbyetnt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxdopvvn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrmjidde.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grrhazhqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghaduewht.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gonvqtxmw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdzhhxxv.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktfjxpzz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gylugpkja.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grdruroow.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsxyihfl.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioyveraa.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gfacawoib.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpoefylxm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijxnugcj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gyrakrztn.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gkapsbtyh.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grvflreco.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/goyhaorpf.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gmndyivrn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwniontaj.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnhovok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gunkqoxkx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmcfhxel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwrosleti.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjozdyid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhomupx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gepugdnth.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gupleibgs.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzkyvvej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggceytdvu.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxqkminme.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giglllhcc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrkikpmh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbscqtnth.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqmkwzx.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gviqtmygv.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpckijltb.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdwhcwsh.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghuwazvwr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjacjlemx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtkdgyea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwfzpfljq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gozhusudu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gttgodqcp.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpgrbhwk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/glfkeohvi.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ggvmkmuul.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gyhmdrmhj.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gotwgerhf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncaxojyd.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnyerezg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevyicmsj.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjizxtquv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gizwfrmiy.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfmxjjif.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjdptcvre.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gloyzcgcp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizxjdqsk.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gfowoullh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gafjzsemc.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcvlkolq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylqhkmh.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/grpgydjfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihzwcti.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/garetgtmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gafroesrs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmzmjcxiy.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzmawwon.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrapjaky.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmaxquvr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdpovbtrk.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbdckaqkp.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gexnoounv.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/grvcgdsev.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjbpyavs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfrzqrh.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gelpyvkqx.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grqbyovut.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfhbgzdon.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomhfeymj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbkhwvsc.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gougosyxu.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlnfnndf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/guwvoyygg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/guapgnjpn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpzlccig.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwmdwfqjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmiqxutj.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gizagunqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxdqakkb.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gusftdzfi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gntzfzftk.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbuhlfgjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfcxpga.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtphxmow.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqeepaqq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjzflgu.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gluukgoht.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gysjjmynn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevzmsff.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gecrzpbbx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpintsrgu.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gaejkwtfr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gtprlgacx.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxucksyir.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlgkpptf.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/grlzvkaac.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqzyfns.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcribmn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gbgiaroef.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnvyjla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeokoxkd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gcccuwzmd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grtllizdt.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzjemupxj.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gmsvhwriy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrondiic.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gaycfiyyr.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcmxoghpk.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gbffgyngn.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyidznsm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyhukgix.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcwvwhxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagxwezqg.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsbomupk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlknocly.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/glmutgyar.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gavmfjcle.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gasigasqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnjzweo.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gyeyrmikp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghspeykmm.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrydgrk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfspgnhu.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/glknfuhso.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gdxvuzduf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmdsqpwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxilrpbw.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkdtmzgip.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gssiixpxl.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gozsiywsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaiyixhzz.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqtkoovxi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gungckthv.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqwsnjyz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpipjgygm.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsumqqpp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gublzzrxs.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/grgqgcrvd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkimcejh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlfvbvz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrfpdfa.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggfcpuodl.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxscymplw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdjongaxb.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrugparj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwdisjsft.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goojaiqhc.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glmlnqoyw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmiklsykl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqscufrq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnkewego.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkccaovc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbdxeobu.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbkbrhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gapbpobsn.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqniengzf.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvrqznj.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gewrhlqth.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcfbsztl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvfnvxbpb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gcceozkhi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gecjevzpn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupbogfrc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gszjbzmzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gicbxjuzp.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gcxmdxtwd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyanesyb.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gutpypgaz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfkehpm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gymrjwvhm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsaqdgck.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlxnkexk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzljbzuzx.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gyijfpfum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gmyziwgvm.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkziuruwi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtvlodzj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwukmbl.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/glyvbscfs.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqtivbea.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gktkirtiy.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmosnfe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpxtrtzm.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvhtxwnqz.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gjqatqemn.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnxctbbay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzeumtozz.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gnomqfjcp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxthdgxqc.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkezzjdjq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gawmnsofk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpirhgqyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkkxpuxs.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gaxqfqawi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gvivxcwzn.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/giglakizg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqgbann.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxggqtrk.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/ghplswrqe.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gskbavoki.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzzndsg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxajrclte.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwydhqbpd.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzzllcggn.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/grqepocbb.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfyapjzpx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/goxwrgdml.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gwqnpzlxa.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanugcpr.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtoonmnoy.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvsmgjv.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkzonjtu.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpifsapli.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gczjzbybn.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoitazob.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmywpjeb.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gzevaqjgs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjwjnnfk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gagjzvvva.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuwhfoew.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/grqrrossz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/garfygadz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjbsooen.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxdjgvlu.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkghurmzw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjjgmdwki.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gghigsbxz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gsshoicnz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwnkbmaa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gswqqcvfs.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghygidmlu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhyqsrtd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiknrzvv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnssabtdv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnlsuoat.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gjmquciwz.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gefzmsfxm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gguxwnlmd.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gfziujdeu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutqatag.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/geqbzjwmd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/ghywowmwy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggspgbytj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvjlquhrx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfigenixd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrxcegcf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnchkixnx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gvhvdjkbj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gczatnnow.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxwljwmtm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gupyydwma.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfxxujjcv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdutremna.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxywsriab.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvqpfaxkk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gutewacre.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvtelrlfw.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbxywmfi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/giavknody.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwflcohnd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtjcqsp.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gupligrzf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gapinhbyk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gslhdvlbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfrzzzww.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskksgdkk.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaqvgucr.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghyepqokk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzudaoscn.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdlglpim.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpehqlbew.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/grhuyghvl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/guxjfujif.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqqdnyexy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gontdlxaa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkycueoo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsahnsjjd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gklbvblrj.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiqxrhqd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbyneoyh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gldhdptwz.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/grtvsmdcp.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gasnmdqnl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpaywvtq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsocugdaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/glidotqdw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gkopzfwgb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govupkbkj.sHtML


<!-- 参考信息 -->