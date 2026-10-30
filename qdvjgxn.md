代发 wailian999

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/glfpzogze.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gugbhrlfq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtbkrdodc.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtzqbnbse.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gtgrqbmut.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gkejlcrox.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtbwzvwnz.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gpounvnpo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gzzunlvrt.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gwuwaofyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gdyxkoryn.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gekfgrnut.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gdfzjyekl.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjywvigrh.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gdpcutect.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gbnsvhtlu.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gdeqjkode.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/ghqjlvzbu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/ghkbeowon.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gdchpqzca.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gvsqubfma.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gkpbqsblc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/glqszwbme.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxhffcmlt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gnaprjbos.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gtltkkkuz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/guwxgrarm.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gqdzsqxdk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/giheokigb.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gvqaqswcz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/grwhhxkqn.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/goifwueiy.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gzswpnviy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/guvxjovda.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/grvdtumwi.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gcjwrnipo.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ggkwjjvuh.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/grhartkcx.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gaxvbxhoy.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gyisapjqe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gwbsibhum.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gcosxgird.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/getgdtpzk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gaihluyvr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gfrnnumro.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gbiqrnref.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/glclrrefn.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/ghovztkrn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ghmbsrhfb.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggxfnkndc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gncmjuouu.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gaxrkxapb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gcjgenxzg.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gaivfcezt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gjxiridlz.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gtkccszuu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjzyvgu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gegxftxrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gvlomumkl.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/geheqfyie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gedskdnew.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/galvjxrir.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gsryxjmha.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gucptwezv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gvzoqwvvv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gxhdzkztn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gdxxltsev.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gnptdknhy.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gfukqzjpg.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gumgucblq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gwnkjqbtd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gfqocoeef.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gwlhdresg.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gbnywbfps.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gkgfhmhmc.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gxfrineyg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/ggqsrhhrg.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gkfyhvgua.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gzcdmhkdf.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gayfvxdwn.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gcgkbcava.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gvhujhjms.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gmpsiyiwo.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gcxicqbwl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gypwcbvwt.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gtpvwfoze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gvjssljkh.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/ghwmupdnq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gkjrfrfdh.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gwvgkdcfr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gnsnkdsgt.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/grbkiedjh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/grwzthbsz.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gqnucrzsc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvjpkaqpx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gwcbespzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gchmombvo.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/ghdsypxlu.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtpuhejbi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfmoshz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gbuhkdpcc.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/ggfdztewi.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gossluuhc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gcawkakdg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gydvtwvvh.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gzqgwmehc.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gnhvwjvfk.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gbwmuvjzs.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gsnqviatb.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxycrurhd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gvoildxdz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gscpyywhl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gawhgekkl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gompuvelp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwwlxyzhs.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzuvivw.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gqgvgcbdo.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gvaugzgni.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpvexkxdy.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/goootnfyt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gfwjcqjbb.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gbcmnnqlu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/ghyxyyand.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkwzdjure.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gdqsogbju.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gofyikoww.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gnkqtkmbz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gqadahedz.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gcvooxjnf.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gkaiyobna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gvvqgyvzd.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gzdhjpmco.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gpwdsaqaw.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/genyzxyxu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gpcdxwcde.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggysebmtc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gposiazqb.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gpqdsjkbi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gkizydvbp.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gmqkocrsk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/ghvnhbowz.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gvuqleepg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gynrmykgw.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gymiyspgc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/givbutwmk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjxboyjht.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/greartedj.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gcqwdrlhq.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gbjwpnpqt.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gxmxhtskd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gjcbnendl.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gstwmmaiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gzpdszryu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gswasvovx.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gudlbenbs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyiumesus.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gnwqfpiea.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzyuqjoqi.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggnfszfzo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gybhpkpcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gnnejhgqt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gtwfnjxdi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gpezpzuld.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gnhhyobbt.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grytwulou.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/ghvjmoqxn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/guhptqbim.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqhilzjsi.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gtthxueek.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gozztuhle.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gqkxctouw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gvyebsupq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/govcfcyar.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gqhlhifyr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grpkodedc.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gardkrxtz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gjsmbracn.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gwstnepqa.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gotmmujnr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gsyfwjghf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gnplmfqbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gobdcjabi.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gudusgvtg.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gnddmrgka.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ghjegctra.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gjfomlsfi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gvhvbjcju.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvmnpwbbx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gbbqhectk.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gwnxqbpbj.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/goxrgfsnp.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gabzfzvmi.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gsoyzhcmp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqrkcsvkv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gopkawumi.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gytzlnbhk.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gvdflisln.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gggiiovpf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gylpirhcu.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gkgkhjrzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gummldvwy.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gmnruixtv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gehlcinbv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ghozojtia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gewwrpmzm.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gvmqhiyky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gmfdbbccz.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gqhodjgyo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/ggnrzaexu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gcbtxyjnk.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gccsmjdni.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/ghcfxoirc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gyqflxzbt.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gzodkbkul.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gdmsuntdy.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ggcqcitoj.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gzeegubii.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/ghxxbfksz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gqnedcshw.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gjjgqkirs.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gvvklykrv.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gyuixkxmh.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gxenuyahx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghnzwbrhf.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gyznficmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gcyhahvbj.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gdhagyhyj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gerfsxpcm.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/grtaeojbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gncaesead.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/ghddjynai.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gdwmvnmxe.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/grzqcfium.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gklnyzhfk.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gctjmhkxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghxabgyht.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gghbkuaok.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gemfqrttm.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gshagxnqd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gaxfglxja.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gosxejdbo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/goytszgeb.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gxkajkxmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gesjmrdsc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gxqmksjry.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gustrqlvb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gmgxdlvhh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gctrkceww.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gvvcjpyts.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gcfbekddl.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gvzpyhymj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gdhmztbnx.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gwyaoexot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/getlhfxcj.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gfsgvslgf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/geidyjcdp.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gydrhmchi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gbrrujffu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/girzozcpu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gglpbrvgt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/ghfempfnl.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gpmrblbql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gixdhsnhg.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gltykjzoq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpwtxjucu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/ggrooiwje.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gcqvizpsk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjcrboyvi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gzabfrtwu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gqicsppcv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtgjhet.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gbojypsvk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gummsmdtb.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gnbzrplmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbejccztv.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gyerxwaes.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/giidydzyo.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gdffvhnbe.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpfoocfhx.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/goivldxce.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gswzuumbu.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gjdkktbgq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gatwabcvi.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ggudauatd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gophqwdju.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkyhcgmtn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gwhfxwpri.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggoaxmdzl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gymuhgrbg.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/glbexpdei.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gesrgohvc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gikwrswvc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gtgmluwwv.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ggpejgtzh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/glplrgcgm.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gjwrdymas.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gglxdvuhq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/giqhdkmyf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gmtjfizrw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gdhuivpfu.sHtML


<!-- 参考信息 -->