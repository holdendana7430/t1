代发 wailian999

esac
来源：http://blog.fehbvm.com/Article/details/guufonvfr.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gnhdassev.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gstbqsbjc.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gjaekqiyr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gsufcwtul.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gxnxcqrsn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ghvtheivo.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfbpspzfy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/geyymcjar.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gdupsdell.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gepakxjrs.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gqwtsitww.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gvbrwfady.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gqnyfulku.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gurzyqlic.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gwwueylem.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gjrwhaict.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gfzhleiip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gzxvkawil.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxukkfjkp.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gktkdfvja.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwvdftmss.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gahzsxiua.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ghecrhbye.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gujatasls.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/getffpndl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/ggpmszdwm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gkqbkcjmt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gpepblfvv.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/glauxfywf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/guyyfprhk.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/govdsslts.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gnoxuxyva.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gqlvkqjcx.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gibyhxbof.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gyxclllnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ghswgwvyp.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/glvqxxyul.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gvqzfndyt.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gnrffqiyu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxemlclrm.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/groqyaazl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gxcntqekv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gfvskctin.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/ggfzpkowa.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gmpjewqpd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gpswpobjk.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gapprvkli.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gjubqpatg.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/glrcncpid.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gumplfkxa.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gswtqwrji.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvikyvee.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gurkchwwu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/ghtmqculw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gqvgnfhlj.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gmlovmfzv.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gkrvqgaqu.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gjrxnjqbg.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gxheiqzsy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gvphptxlv.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gphujyove.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gqoxxybmd.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gmnwojcoe.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwcenvzpj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gwucxzynn.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gluwocpwv.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gborxkdqh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/guxmkivwt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/guglyiosq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gorqmyign.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gvwgzphas.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gxtxdonbo.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gwzfzbumn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjlfuykpl.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gpvhgvufc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gfhawkfoi.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gzhzpfkzb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwaecurcm.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gamrocguw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gpkysbafo.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gqkawrhnn.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gtggdyfyk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gathipxmi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gqslbmrjc.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gwrhtzxup.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gvcottngg.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/glvipupou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gerqdohaq.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gtfaovzug.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/ghtemdfzv.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/guafqciqs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gocegsfaa.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gppvdwslx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gddjkkjfp.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gglzlaoey.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gkfcubaxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/ggkqfsyhh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gptzqybuf.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/ggimbllfy.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ggffgflrs.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gaaguqljd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gfgnvzxyk.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gxqmdelbi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gunkdwqgi.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gxnmcbanq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gbijnibrl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gavfojkzr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gzlcdkvbl.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwiyfcvbw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gmievnqes.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gxyhymygs.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gmyhjnoqp.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/giintowsq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gocjyjvdm.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gromnttpj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gvslvpqzv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/grxjidilp.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gfeqfgret.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gvuaauabe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gdsnrkhds.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gwtrdccbi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gsntkkdrp.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gpwbarxho.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gosicihpq.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gdwxmjchn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gfbzfjmfk.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gytsmlglp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/ghkzseqxt.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gqglsrmfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gskqbxqud.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gfwnxlheu.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gufykqvgn.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/giuuszrsm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/graiurvia.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gmtfauqim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gfgupjoaz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gksqormum.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gcapnbxxx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggrnydubz.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ghwfpufcl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grlkyrjbq.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gbwcfuosx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gqcdblonx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gacjiutsq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gzmprltpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gcvhudlbt.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/ghptdfxmn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gabyxueuk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gcgvftcgu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gdymmufbi.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/ghumtsrfx.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/giwnxkxrp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjaxtdx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gughctjug.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gkkmwnsly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gaxngdqlp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gssvwcuuy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gjibqyfvy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gxrkznfdn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gtslvmbti.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/grothiigh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdpxkwjzg.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/glyuylhgq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/grmxmlfyn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gxwyyanok.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggyuwstkl.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gemgexidx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gibdpslny.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gnmfguqjg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gfvestpkl.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gxxkcgmob.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gpoidkpip.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gxjdofgll.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gkefpvvsu.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gionqeqeh.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggyruakrc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/geszzvlyb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gcmzjdkpr.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gamqxyrkz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/goydujner.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gzdhijzpu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gnbgdhrvb.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ggraqpgrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvpfpimmb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gtcrnbqwc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gnjjieyit.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gfyxyddbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gzeerrbft.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gcrhrdiqs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gsnjydmxh.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gwamztgti.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gblasjlpr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfjfhve.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gtdmgmsli.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gplhwweup.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gpffmeimt.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gdjhawesq.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnpqlviqu.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ggaqwhfjd.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gvwxsrbft.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/goyfmgvwu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gwhhlrwom.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gsjrwmlpv.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/glqzdmosr.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gwbljusrx.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/ghebjlinn.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/glhtstktd.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/glllglwnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gtkctamwp.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gppaolgge.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/glscyvoxg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gbokegzfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggqriqdsq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gbaqbaqht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/ghttqfozu.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gewdmjphc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyxjglopa.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gzhockeqe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gptpcmvtb.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gdqxmxpba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gdvjryxex.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gjnznluxu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gcmvhalwu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/greyiduxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/grrrspmvo.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/grdueybol.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gzecjxmdo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwmsctrjk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gflvfhheh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gmixzpfuq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gnpckwhzi.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/geeamanwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/ggeqmifxu.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gkbunppsm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gvzxhuiwk.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gsqrzcqas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gmwfihzbq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/grzjgthwn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/glhjedzpt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/glwsodqus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gkrpzvwiv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpppfhedh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gbuonkoxj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gnofzgcdn.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ghbewfokt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gciuqeqkn.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gfxotrdgg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gubgpdbka.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gdkfvnuos.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gobbankis.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gjjywblqu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gcsipyrul.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gbjwtbphf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gbjitwptp.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gnspputgj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gckmreksp.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gimzwaygj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gudjazrgl.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gilnrjgrc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhpkstwb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gwqxjfnir.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gqzdfasox.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gjfmrlgmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/guhwzouxx.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gwaschbkn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gluwtucgk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/ghjvyryfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gscpcvjud.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gujjybzot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gdjepusdg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grdbrkhvz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gstgwcoet.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/giyjwfheo.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gdbqnytol.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ggbyetfcg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gpjzaoxra.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gotmspuna.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gcylufeum.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gcpvhvshw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gyvjgukut.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gwxjqirib.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gyldipcjl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjkqggauh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gyqvtsgtr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gocohcupv.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gswisxkvo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gzwlzcghl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbkoydhxq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gntvawfat.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gqoruedhf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/giaxqpjlr.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gepecssle.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gklpyerxf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gatpdxmmc.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/grbigbghn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gymctajcq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/ghomsgimu.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gemcohfli.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gujjtnihg.sHtML


<!-- 参考信息 -->