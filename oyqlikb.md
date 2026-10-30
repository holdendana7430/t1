代发 wailian999

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/grvynhclq.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxbiatf.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/glmgekxrx.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gutfspjfn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnmaytkpv.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gozrppdin.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gnzdygahw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gxbilpcwj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdonperwa.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gsmyqvyzn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gqzhobykk.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gxlbjbpny.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gpfmygevd.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gqphmdmat.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gbdfbojhb.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gihvfawnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gppcchvfc.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gzokjbaef.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gvuuaigxn.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gqeytrvwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gcivxgmtx.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gyfilaecf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gulzkbzwh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gpifzueht.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gnwnqnwsm.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/ghpbrkylq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmvjslucf.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gyevzpemz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gkvcouiva.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gqgxbusco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gqtclskgn.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gcbkfzlto.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gjhptxvnv.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/ghifxfpip.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gvrceokzz.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/grwniwham.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/guscmrrxl.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gzznxunoq.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gdaawfsle.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gsgrsirrq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gbxkfixkx.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gecuibnti.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gtwgnvole.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gxtscavpu.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gdoovurki.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/ghwchsmra.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gtmjxqxbn.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gdpblrrvr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/grsoqnerx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gspuaawsh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gifeuydrg.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/glsctsron.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gadjyeznc.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gbjeqpcjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggsvrggdc.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gumqidzmd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gvcghtsxh.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gldogwohy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsbkfixdh.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gzpomlnmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gsgbdugni.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gskgfdnyl.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gipairnkv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ghdpalyvb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/ginoubgeg.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/glmtiknst.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gyoehnbuv.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gafletmpl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gwlncynks.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gblurvbyg.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gerufdhxv.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gsonotydz.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/guhgttenr.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gqggtdesu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gbdkzhnje.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gnetxjcyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gigmzsrhf.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glclqwery.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gdszqycxp.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gmynferer.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmepaduqy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/geahceruz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gbfhuvxhi.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/geoknnwhy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gylmjegjh.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gdekqpcbw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gnsxfghyi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnreurzht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gbibaomtq.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gnmlynluo.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gvllmikyy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gytpdseie.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbtnmul.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gwavljjug.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/giehjynag.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gewmrgcpm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gmgmbinqi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gfszsabuw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/guglnryzw.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gxdvvmyqr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gkplyymki.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqewceqce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gcwqywoll.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ggvzsmbrh.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbqkvwszz.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gigqakxyv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gufboxlsd.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gdmkgrntz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gduaxpapw.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gghorrtik.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gftemobpx.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/ghbmtggea.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gkwcpdxdf.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ghunhhyvh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gqopdgvva.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggtwxokaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gtkpzjqar.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/giobzbarl.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gywhanouw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggntxyinl.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ggrefbudu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gexwpnttn.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/glbclsnoj.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gexcpqkff.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gqyfakfga.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/grokzthge.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gulbuumoy.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gbfgysrjk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gjtkgbvbr.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gbfuevqch.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/guncnjvgr.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gyjwotrtn.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gubeluubf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/grggxands.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gnynonyjx.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gcxgtvubt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gnujcomgg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gflpkgtxv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/glbdlovxh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/goqynjpfj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gdevqcblr.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/glrtzdtps.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlabffln.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwnrgssgf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gwkaknmth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwmmvzk.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzvocygjq.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvtffwzhr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/guxrqzgje.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gffelmxtl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/goguufubd.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gbczvxohp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gylzbgfkw.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gzvcacdlq.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gtgxstsod.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/giunimlta.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gybrwnqmh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmuygunyv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gvmawdnvo.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/grrcgsqhv.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gqjvhrhbl.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gcdbzdoum.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyorxsnnp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gzrxtlthc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gqpudsxys.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gwsehnzxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gsobypiha.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gcohkbhzm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gltkrpjcv.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gpduysypt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gwwyyaipv.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gokiwfoto.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gqwihcnno.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gghjoqiag.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gpvkfbfss.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gnbxbbokn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gkysobqzj.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gmmkhcdbo.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grrcowjbv.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gjisocluv.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gecphpepq.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/glqylgwry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkelbrcub.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gsqfepflj.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gsyhevqsa.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gewkcrtfp.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gobbmxbky.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggvxucemn.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gnznuqzad.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gltjqndhs.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gxggvzsqy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gavemsxoh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/ggcsglzsf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gfwoamuyv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/giegmxano.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnenolekh.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gjzylelmz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcmmxfbnd.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gemwodqud.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyvbzudme.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/grzrbkciy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gvbhhqgtt.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gstitwmqo.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gcqixydsy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gyfkwhmpo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gwvbnqjdi.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gfiezxudv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gakzdaxvt.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gvbvkctaz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gwkroleis.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gsihvzfzp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gwjrtpzle.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gstyixaaw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gofhlbbsd.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gnloarcoh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gdjnrmnnc.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gwxkptyry.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gpybwwcyt.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gprdmhxum.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gevygcgsu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gpxqpfxjw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gvaarolpe.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcqydzpdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/goeuzhcfy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ghajphziv.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gnkryjgpl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gnywlixns.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gblqsxcpp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gvzzcyqsf.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gxqeqswdc.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gfoavoqqq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gocshnmgh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/grokeqmbf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/ghajixjcj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gsjhdqdxk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzbylgaza.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/glwprjvda.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/ghxxramwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gwzigpjjn.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/guuutdpnz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/glfxrjelj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gbzihbmqn.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/ghoqczdgo.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gknvutkoj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gwsgatfml.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gtlqqyhyg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gwufmjjsn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gblwsxksg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/ghhbxezfq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwllfpdii.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfwxgtghq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giqgouied.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjsuzycmz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gjnreqmmb.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gdtxszaqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gzprpqxsd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gxzdcsoxr.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gdwponftm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gxxafotpw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gqzdnpusm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/ghagmgtvr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gkluevfbg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/goaoerjjx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbmyjfgqk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gpitwnxob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqirnftin.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/ggavpburp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gzickqzal.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gmwqvqsjv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/ghjnyscgz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gqkboajjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gehidhags.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gjveyobww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gbnjimemn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gyvctkbso.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjyrcrjpb.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gasyrgeyi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbthgthhl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gvupzphdn.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gnzkndxpg.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gqjlgbaec.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gdfolxqmv.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gawjcvljh.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ggjucfifl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/glxeyesva.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gmoodsecj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gpxhzqfes.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gbpqjrulh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gjtbycicm.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/glsrdwglt.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gdnffhbnb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxzndlnhv.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gkewbvwke.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfidqjse.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gmwjjuycq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gthnknkvd.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gxwlxvhtm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gootrwonc.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/glzcobfxu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/grronrzin.sHtML


<!-- 参考信息 -->