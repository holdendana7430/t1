代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gkfwmdzeb.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gbrjbxldt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gwwmjdcil.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gdigcbqac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gxvsyumpf.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gzgcaniqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/giyxjhlci.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/grftshyec.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gtekdchpt.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gkwhswles.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gllvzzllp.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gyyrzqjmy.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gzxhcnrsd.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gkgdwwhej.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ggreihxgb.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gouinvjsk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/ghhcckoew.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjvuoulfl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gyrtirxzs.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gniqrqxol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gksqlpeuv.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/ggzdkfert.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gkwdatsbo.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gfeebpwgb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gesibsynw.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gzgovmmrm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gnuxbxpye.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ggcfogthh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gcuvyuvxl.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gxepjmuhr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gmslzwypz.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjqnhqena.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gvupwhyuw.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gatlbsdzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ganmycbjf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gtpomcdwc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gblxmrfgq.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gpdoeptkk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gykmawwpw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvqbwokcl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/giteftmrp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gsbyffjyn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gbuzcleem.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/glvhobwsa.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gtknivazs.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gdzwaioxq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gnvpketdi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gvamrifmq.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjkdpdcve.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gjlcblsee.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/geluomyoa.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/grurjaqor.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/glrvohkvs.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gekjflvqj.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gawxqqpum.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gtwrufwki.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gucixayvj.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gxgnhayii.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gnxpcvsud.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gzqsqwrcu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gvuouxxah.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gxkksjsgj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gafryiahu.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gmcnwhacs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqfcpslwz.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gmmfderej.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/grptqhyrs.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/grwsgjimb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/grzmaihht.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gdrkugxlr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gipmifiqf.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gbczfugad.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gpbukhznz.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/glkytjupl.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gkdphonqj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gzjnodhzj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gmqcyfewj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gqnosajmj.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gmpughxuw.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/glhbpbjpc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gdklsgsvd.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/ghazxbvnn.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gvvdjramx.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gufknnupr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gwjgqxjsx.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gesyhvhec.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/ghspracrt.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmzgkdbno.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gzmkqbtmx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gviowzvwx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gfcfkfijk.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gynvjgdpg.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/giwfxfwii.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/ggsavkyrd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gzwaaoopa.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gfyhuejgj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gparksazn.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gpdynfsch.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gyplhtfrw.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/ghinasryz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gnvmjafsc.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gsimctgsi.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gwvvxakgo.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwqkqio.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gzrdhazql.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gwlthmotj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/glmcqyxny.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gykqwukjj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/ghzyfpvli.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gmxsfygxj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gaejghsrg.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gutyvupjc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gbmpepdov.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gthinfzjs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gutkdsdfc.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gcmvwpxue.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gctfsztjn.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gqybyrloa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gyfmfhssj.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gavukdgqe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/glurlyxld.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gqhlhuuuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmvimxqpj.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gotdqksfe.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gfqxezbdq.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/grnlehtzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gymbjvnqb.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gagwwswnu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gzxolxwya.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gpmiholuk.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gwlkfmyjt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goqfmwvew.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gntjggaju.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggxqnmoss.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/goywtwmor.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gbuzomxgy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gtsefoysh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gwgddvwgr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gakyendfz.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gsvvzutwc.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gyddxojlb.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtoyinxvq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtvfowmrv.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gtvjmwawr.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gjomibbsu.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gcigdotwn.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gaqovaiyl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gyzyvrjtp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/ghjdqrkkz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/guwxzcrko.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gjaukcgyy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gunjfjjcu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gxiuljrxq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gawyejuec.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/glgtrjmyv.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gsvseheza.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gdepokxcj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gebwarnwz.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/geckijays.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gpxsznfwd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gekcnftwn.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gfriwnlci.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwftyetlp.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gcsxicopy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gffszsvvu.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gttfzewni.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gsghgdgrq.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gqwtuqyms.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gpehsgmhy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwfkwdjgx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gycixplvh.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gktklbzlp.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gwmtiussr.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gcnuoauwa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gazwazazh.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gvnheuqov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gipupucdo.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gzoazitji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/glpbfsdln.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gijahemmc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gikivlvnp.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gifmyjdry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gbvxcmdgp.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gekkhklzu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmiecfijx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gywafhmch.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/giqbrzsit.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gibanidsi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/ghiolpqgo.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gxkldgsqq.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbnoaocwm.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gcswqgtue.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gphytbcos.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/guoxpymiu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gmtsgylej.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/glfvtiyji.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gjuyhcsra.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gfhjstqfl.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gtllqlrgd.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqxnmpusb.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gxuuftzvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gyleqyzln.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gfvtefjao.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gxzntgqni.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdhbcboaq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gmijkhuka.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/geegapqdu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gmalsfcim.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/groxqgzss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdlgwjjsd.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gafamxsul.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghhteortb.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/ggpnddwyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gdvyhhwvz.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/glimtyrrb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gdwxkfsat.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gexqbzoxo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gxvogiuvm.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gqbaehhhn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gpfmldyig.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gdbsmyhue.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gozzbawfk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gaeomojns.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/ghdyyvonw.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gqfjtoukj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnfbyve.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gvjqsxjqu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gqgatawvy.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gspopgxen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gglvkdydh.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gtkptxmep.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gnrunfbqx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/grdbjmktk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gepgvbwfl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggtrtfmle.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/ghmjfznla.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gphjtrbth.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gnukzdwif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/grkjgxmxo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gkgsjvkhp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gskorlxee.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gxpnoqkow.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gkgxazyzr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gifwfsxwe.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gijpekukl.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gpxbifkig.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gmrjgmgye.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gpfgrvhel.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gpqadgbnw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gsscltsyh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfqktqcxb.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gkzvffiow.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gsweldbsy.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gcibxzlvm.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gctlxusdv.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gsheremtc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gxfgswtqu.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gsprfcieh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gzqethemn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gsyndjwye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gtntbzxbl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gajurlpro.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gogygnjlb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvczustwa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkaicsubc.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggkqkhhpg.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/geigijlgz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gdoqospgr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gfcxifdib.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gzznvcesq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/guefgehzn.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gyzibecir.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gcmewvhbu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/guyfjotuh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gzjstguoi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glyuaczvh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gnxudqgpx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gdyymaxjj.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gogxlkbnw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gqhgzosax.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gnxxeclhk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gruwagqbk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gjbqjcxem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gjnbqswor.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gzjpvpnqg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gzkxwhbys.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gqztrcpoz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwfrwygfk.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gpktcnkcp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gsuisxsot.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gfnbxhyoq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/ghabviiik.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gjbfrbbrd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gxpdemtas.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gplpbemjg.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gyycwpjkx.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gmhmsxsgz.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/govdklrwq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gpqaqsodp.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gebuxnuge.sHtML


<!-- 参考信息 -->