代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjaivzsbe.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwosyhdy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbxeper.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gzdjumajv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghhubkjig.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/giyganiyc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gswgjcwjp.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwgquuva.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gxmjopjho.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gwknrqtrh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gybjnsfpt.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdhycokq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmoptfliq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuiekmcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvfdazih.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gctxsbeyu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnsojuhu.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gplsxpolr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoijvvex.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjhbqgy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gussrwtyc.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gfteivpke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gygekrffn.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gcuknhryj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gianeikld.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtajvfhre.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gzqamfppe.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwccmgrvy.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxwjagcoo.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvielcao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gkeocjegs.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gcvdptakx.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggrtjkxdz.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gudssnmnx.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpylxtooy.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gexyiimtz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofyikouw.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gholtztkn.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gysuryfba.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqqhpddgu.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuhqkisc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjbbgset.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfcafwqge.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevhilihp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmwigdgx.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gatnvjulf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbxmwhvd.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwvhygqia.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlyddlqd.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gfkiokrgn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxcdglt.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gofsbmhvi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gccnrdpga.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/glunqvdvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrlyztga.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqyfxzjr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfyoedbi.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpnsfghsi.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcllylxq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbqyerx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gsoqdaflh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcnsrjlbj.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsomplvlm.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmqqaig.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ggevakbwb.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyisbijht.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeauwnbi.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gsyazifmw.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjuyafllz.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfohnnprk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldwanun.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyitsbaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawysslpn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygsaxpkb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbiqewyme.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grnomkbzb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/goguvsgxg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgbdssqi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gmepsxjmf.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfymoyxzo.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/grfryuvtx.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrzwpefo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnvzwmeu.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuxskuhw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdekljjm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ganpreukg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejrrdqe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkpoialm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxcjaicj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfglsiir.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckfrzjd.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gufpplbbp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gezujspig.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdnsfnrs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gxzjzcjym.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykxuyqmt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/guvulcivg.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqprlyjz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxrwvsqs.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxbvwbkmg.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gayhdhwgy.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoxjoqdl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmogkaec.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubipmmk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjdrzsgl.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gduykmhvr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guzlzoihl.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gkyxlvayv.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gwskfbipj.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gdmntjuaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxjtkasz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gyolmjldy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrefeqtt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucmhqqu.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gobbcwavv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geeyhjyuc.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvncjuqo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrqpyhor.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjfbnhzrh.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhrkuosd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejacsfea.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/grxbvnaaf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbqxnxwyt.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyoddjrt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuktsfxm.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gisowdijd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiivadgz.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzvowbfo.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahrhogxu.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqdkkujq.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gjjrvrvsh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gllxcjvhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/garxzrzcz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gljfpdvtr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqjdqfix.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskartgw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gowglklyv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gygtmoswc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxytbxlr.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmwqxxhfs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gqabbanzi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbtpynzg.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsoirpzg.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/genqfishp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnhfpggb.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gvyapimfz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gkkocwjhl.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfkefqpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gsgtxzhay.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkaazyxt.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/geffuxxif.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoeylrco.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsakwqeu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/guwfdvlmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqhszbd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtldnpnrz.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gypftpdoi.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjwynsag.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmnenqgvj.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggofghyum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gpvhfbqtc.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/geedmapli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeqbgixi.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gligzhtwu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gokxahohv.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gypwigfut.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gzsmadxch.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmvetglff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmmhasr.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnvjoseft.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giivlgjpz.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhwefpxj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmpdbayv.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpjqnuwq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtspawxtu.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwvivbmip.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnteteryu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/glstflbky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtksoskp.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/glcdscglx.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwghgxej.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ghempejxn.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gruibyuoj.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guhdemjxa.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gvfamkphr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gciixqdzz.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grknrjhxf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdaxolnh.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqosyuc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtpccjxlr.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gtcpkmcpr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkulhmkoe.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhcrhlfo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonvfyyz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqrxohv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfguenoyp.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgmhvazg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gruwmdhps.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gywsprfxh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxhodpmxh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqnvzqla.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzulziasy.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gptykdwqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpghbnulg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxylwgkbt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gczpnwocz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/glgyrdqef.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmtyejer.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gffvyelip.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpfzmblx.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gmoesyczd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvqngihjd.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzvfgkpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gauckhfeu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbkfkbqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gktkwmvxu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxmqhskbx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvyaujmzi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guphfntmk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhahacwa.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqhdydxq.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxriixgic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gxyfvsxlk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbsuvqj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbkzooo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvnoceq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyaabklq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gjegvfbno.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtoznze.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gukegxnea.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebztteyp.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gtscazrin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxxinvhs.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgtvifm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbtzsros.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gjrasblfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfvmjvtr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatntllot.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdzqjseu.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/grtbpdocu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdjflrctx.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gglolwkod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuinekkw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmvpqxcsr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gkfycuxqs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtveyvpsq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvyjfgxz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfukkfkcv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gonktouwo.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzprocjzb.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gacoqxtjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gpacpnwsn.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmfwdzhwu.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghfjigjel.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaeeabzh.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gggfxxgpx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmryhmmea.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gzxjcrihv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvmxnhr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfukjerjn.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gedkjtthy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmcfwybn.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gkvqzeuhp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdrlwlhx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpttwjigk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqucnat.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/geazragno.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcapalsmi.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gozvxvdbz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwcpazp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gasrjcdmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gumuofrsx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkjwsord.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfozrlfx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbdrltve.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnosplzdy.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxdfveaui.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/givbozeqw.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gacjbzssi.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohgcrpcg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthzdjcz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltdbbtnq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzqkwls.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxqokyl.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gmogkwtgf.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfgovnrlo.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxinjcyo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gutmzdpnv.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwpdhfvs.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkvvtpyi.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtswzum.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gldrbzcnz.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gelluacbp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkrzagayd.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsapbguo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrcyzgpm.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gtgjljgis.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxctaqiyc.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtlxlrrl.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gztrnbjwo.sHtML


<!-- 参考信息 -->