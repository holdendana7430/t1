代发 wailian999

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gcdfveaue.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gpjapxsis.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gviruuaau.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gpfbnwyct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gnsqpfgnx.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gsskeinmd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gcalmrlnj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gmxjastes.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ghfvmtlsl.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gaspfkxwx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gydzuilyg.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gsyepumly.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/guzuuznjm.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/guoitkxvk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gxznbxsgn.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gduclunkd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjpwgsrrn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gqditnohn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gwzqbhiuz.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gdtlpwouz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/grgnafnct.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gholphpuq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gzdskqmgl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/giigarrul.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gtqofwmfi.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/glltfuqse.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/grskigxyv.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gghiklowg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gzznyafqo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gkelfqjhy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/ghbbroszz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gcnolymfu.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gfadapxrr.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gnexixsft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/guohwfmig.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmnbtggou.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gbmboprdt.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/grbyectwd.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gycmtospa.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gjlksjfih.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gvffvazaz.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ggzouxbtz.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gpdcuaheb.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/ghzbbguwa.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gswpolrbu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gywigocae.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gepneuzxd.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gswxzbfkg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gwacpxsju.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gamtuoajh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gggsgcxzg.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/ggbeaxfsv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/golxyzzqx.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gghjlgtsu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdruznhvd.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gniebutjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gdlbcwhsp.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gabdpcdob.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvnudyioe.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gnvpgmcwo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gicekolst.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gugpolrhg.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gjkymjmyu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gcaygfbzi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gkpxgmrav.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gqpswgxec.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gewvgfyyz.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gwaycaugj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gimdyihkn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gozjmyvbe.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gbznmaxco.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/ggtctszvq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gekyijvtd.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/geamsznds.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/grgwoewxu.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gquxjyapy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gmqwbwusa.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gdcgjdfxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gratadxqu.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/guahlfyzx.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gglocgwmd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gkqmryqtp.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/giifbuecx.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gdfhrdapn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gxwvozoqv.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/ggclhxgeh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gifwopwcv.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gozhwoyrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gtycmgcii.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gxmxpuqmx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gjceztyee.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gdmxrmskc.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gncyfllof.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbliigf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gabutaxff.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gksprzvyw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gticmuwwb.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gfpxnrbhz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/ggvfhezfo.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gpofstvfu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gqpmuahzi.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ggfgrgnfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gkyrwluda.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gfhcgbmbr.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/giayqkpdz.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gwfzpekzo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gvcvhfuwt.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gwzusshzg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gokywwsdf.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gkirctfzm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gxqnipfci.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/grtiyxvqq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gveqolaqj.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gvgkouish.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/ggacyjwpy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gjjumrzds.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gzwnchqpb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/ggbzwbezy.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gfakipyly.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guuosbgdq.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gwjvopzjg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfqiugvrw.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkehtntjt.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gxxrspvwt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gjphebjkh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gmitjxugu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gariqmfug.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/grdelbaxv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gsetlxcbm.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gexnnuxpx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gtxryrbdt.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gvjvacioz.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gokdpmetu.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gzncmcfuw.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/girzuqcnb.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gefhzghxc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gwvsjpyjl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/giuvtxnql.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ggsmysqvj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gsedmsidm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gfcabaenk.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gqlltzokp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gfdktneme.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsqjaetit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/galtrzrza.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/grbevkfea.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gbpopctzq.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gdalxpwvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gecramvij.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gfdnmqkic.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gwsrvysfo.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gxvtwcudm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gwzfznbda.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gspapzmgm.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/grelyczwm.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gwqsdtara.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gibsaorab.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/guzefdvfi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gehliusxl.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gkzcfitcv.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gywpfapwl.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gcrqnchdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gpwgbtzga.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gwmawvuwn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gentlpyaw.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gznemtynq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gxrjdwplo.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/grnkzwjnn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gapkopgle.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gtqytbzqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gdgiaraxa.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gylafvbmh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gimwnbghb.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gwwmwkdyb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/giupzrmyp.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gfafumwqt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gtpqzbccv.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gqxeubsqj.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glmlaqtus.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gjnpzvmkg.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gdekpwzsr.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gtwtcbugp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gxctzwnbr.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gfwqlfrbj.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gggdvrhmo.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdvifmp.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gnaqqdnnd.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gdqsizzxk.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gobwezrhj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gcdmztojg.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gszjpavcy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/ggvsuqpcm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gpceowdyu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gxkhewcht.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gunrwfvgi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gzftbgyos.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gjgaicrsw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzodgnyem.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gipqbnbip.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzefkktal.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ggmqvzvyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gqqndhhgu.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gmvshpdfm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjfjiemgm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gufinhaig.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gtvedrtye.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gvstilysj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/givsdlgdd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gasjdplts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/grhzgkjfv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/giyewknif.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbbxowqlt.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gbxrssuep.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gserwiird.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gkwlfcaig.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gqgsxymlq.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gzcuzxayn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gdvpazkaw.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gjrlkhvrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/galxfhwfz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gwzbvzyee.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/geosyggaz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glusjbnpl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/geapwurpu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/guiqdscad.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gpxgiizsg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gqqzsajgn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gztgypcvx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfokaczlw.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gvzzaxrhc.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gxsbayoie.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gocvdagcf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gvowbrnqy.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/glaojhupy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gggunlnqc.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gplbfxbsp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gjppgmgqe.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/garolgosw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gizubmntf.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gxgkwtdgi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzzzhwgqi.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/grhcejxyt.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gupbizugm.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gbspawhez.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/giwsqpqxh.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gmxwuicsb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gcrpqjyho.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjhdniguu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gdazmmlbd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyypwtmzb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghknqbodu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrxhbkzk.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ghrcntkud.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gilbqqfzr.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/ghpffckuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gghkmrtjf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gjwowkrze.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ghntverji.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gkqgdezxe.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gjlywrass.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gkoxpwsrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/glfhjkbkj.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gbfxalnlq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gacqayzzt.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/guomvuouy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gpeqlouqk.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gllgcytkd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gziisftmq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gekvapwhz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gjecbzizk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gcolxohxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gyweptxgq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/ghgrwvtjx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrhwves.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gyrsfizzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzlslrvis.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gmdpzxaco.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gdqcvtrwk.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gxiugbbgr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gcocrbcms.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/galarfnwn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gnmyohcwp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmvwptxnj.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/guhgtcexq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gnfcuhngl.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gbdmhkyei.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gdsctbkwk.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gdgcnefph.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gqshqkadc.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/grwsvnaee.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gxswfhqcf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/grozutuiy.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gipehsvcq.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gglqduxzw.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gpkhrkkqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gqesacokt.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gsldscxao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gqxqdctmp.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gmioothfs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gctqwtpjf.sHtML


<!-- 参考信息 -->