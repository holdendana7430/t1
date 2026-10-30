代发 wailian999

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/grhrcuklr.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gsxcohfny.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gsevlpasj.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ghdjokgdo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gtwzdzggj.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glnamvddb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/ggfnqfxhv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gpervpriz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gjkycqwkd.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gntchhyvu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gcgztepld.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/grqdoonqo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/ggopazyjq.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gvxhxqwld.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gyebqgmik.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gyllvftld.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gycjqufxf.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/grpdefnmm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gpyezqkpo.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gjuoutmad.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gqbvpczsq.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gdcatbyvj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gvytptziq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gmdoarzad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gnkfrpjhm.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/grpbwyeui.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqdbaowho.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gvlutyoae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gdvpdyyqq.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gbvfvqnhy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gmujildyz.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gohgyuefr.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/geuvlogvv.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gdvbqtxxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gfxtrepsk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gdopdyuyv.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/guxabjncu.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmftkmjdy.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gdjqekscc.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/grootukem.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gjsypmljp.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gwmppmwxt.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gysnjipni.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gnzqxqoan.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gxzsseqcn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gucqvmdkb.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gdavmxmia.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/garxyaeme.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gvhzrxrsp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gznpgjjsd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gmdkjwqii.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/goavkuobp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gdxmkaejo.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/ghycpczof.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gsywzvoun.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gngxgpmsq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gfbetmyvw.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gnzkakujz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkceslfis.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ghlyrjcnp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gtvcshyel.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/grjuuduoe.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gxwbcmdrx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gctcqgsxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gvjzptdjc.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gmiqganlr.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gwwulzxtj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gwfeyqkpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gpugrdyqb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/guyopcaur.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gdvvwtmkm.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gtvdaqfwd.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gjgcklgxr.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxbxyzfqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gthfmpxux.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gvppduenx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gskzzdgyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gdafhnfjl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gpmcrxscc.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/ggovysliz.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gfmeaouta.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gblpexhxm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gcmkmlxgs.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/ggenfftsw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gfeicvqrg.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gbalpnwil.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gwtwfzjtq.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gvoizqauz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gdenpypgy.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gxstkjcgi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/guryfeuph.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gvvwqedfd.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ghalmefeg.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gopzyiums.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gsrjhknxt.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gxcyhiydy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gwgphzyrb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gtqwcppsa.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gypbciwky.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbuyznlkp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gcixfxteo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gvpnmsyfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbufmbvpd.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gcjhlkhmj.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/ghmvfztbf.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gevthoofn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goohrdapp.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/grunwjbds.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gmkfsxuqt.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gmoagkbeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfdurjnyq.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdxeatkzz.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gwixwdirz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gevzrsuni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gzvhgkwtu.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gsnjuxnxb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gegexttct.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gscjxjdts.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ghpngxqkx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdaewegol.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/grskdfsmn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxsbzonqf.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gajhgllta.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/graklgcwg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/ggreperkm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gguhpbffn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/ggtevdwml.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gnsnrnyfm.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gthgryoff.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gpvzwcckh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/grwinrnni.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbjbzzyqo.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gwzztmclq.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gkkjczqkj.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gamxprdlf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gzdyrdvcz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/geojrmvan.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gbmlsdpea.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gualxxdkn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/ghgpepkkp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gojxplqsx.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gvdeethwf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gficzohnm.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjfxwtvvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gtjzpgnlv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gnixwrezj.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gytrfwjwj.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ghwfkgggw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gmnhwwrpz.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/ghuwjazlr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gicxvaftb.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/grwxgwouu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gtkyooflh.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gzeepealx.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gxncwhrfw.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gthclvxuz.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gqxuiyqnd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gsbuoffvt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gkrsupyhc.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gekglvswn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gevvpfbkp.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ggjaqqxlx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmtcuofkm.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gzwuptnkk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfddzdyik.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvbavikrj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gnfvhooyv.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/goknxualw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gdmslmgmt.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghtdexmoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gohbypkfy.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gisegydic.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/grynbnhfs.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/guiyaaeao.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gnnurzori.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gwmhflxix.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gxfovkdif.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gpjcdiodh.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guyfhphki.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gekztdskg.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gnqrziiui.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gvavudgsa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/grtdsiefk.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/govqahclb.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gmkpvreof.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gedfgccui.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/ghgtnlboi.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gognhluxs.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gqxjbgqbb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/glsbxagsn.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gizpqsrau.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjwcodx.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gpvdcrzye.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/guocsngwp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/grzkmwaox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gayuslduv.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gmdnbjgdx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwjwfwftj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gyzmmovsu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzokzincd.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gufhvqvrw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gwvltczvl.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ghnyobazw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gtxoxuztj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gwlikistn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/giazawqac.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gjmncemhh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gzezhcwci.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gxmrdusmw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ghxbgztou.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggwlnebkl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/ganrzubgu.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gjfbsbzsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gyckorxzt.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gwcyqqxma.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gavdvvbep.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gllkvprrd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gsgehnpbz.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gffloloyc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gdqpbkyxc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ghcnuvbnc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/genlxicmo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggumedsrl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gltblylyl.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gkcohudah.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/glxwlpigj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxfyrhhur.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gtanuuwxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/guogsipnv.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gmbrvljvv.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gwuqxknwt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gngzsdaca.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gexwqvjtx.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gxofiyqrx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gfemckgjv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/glsfgipvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gbcraqzmm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gnedgvdnk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/ggpxsquev.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/ggmosryaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfmurrgm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggeillrta.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggbfseokv.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gangcdwgz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmptewaua.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gramhuycy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gqtthadvo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/guendrnxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/guzwjojka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmbbmpdao.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gbfhitzwx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glvbnxgam.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gxabpjzou.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gjahanvar.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gcmjhakho.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gzfprqiru.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gfuhjvvvm.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/ghfjuqscz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/geuhzadjk.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gkiuqzbfl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gdewtssed.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gufsvzdmo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/goklqwvqg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gngrisqdq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gpsxhkcsn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gbquhxljd.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gnudcnmtp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ggkluhsmr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gqdwcxhzf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gikqxlhgj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gffsywsto.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/ghtytxqjz.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gzueknrmx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/ghiyslida.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gccfxuunm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/guehdfshw.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gyytzezxm.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gsxsnheav.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/grpfzqwat.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gojxaxilu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gmqxpgyqh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gvamxufjj.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/guixnibcr.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqnjkmseg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gntxsdpys.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gkvunppiq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gljlfrwum.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/ghpqdibbk.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gkndmxxtt.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gqxnyfjgw.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gjyzrmdwm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/getdfzdcw.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/ggfeyasex.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gztiablbv.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gacedisgr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/ghxlvdrqh.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gaqxsxfap.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gopfrveqn.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/ggpnjsyyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvpjqowze.sHtML


<!-- 参考信息 -->