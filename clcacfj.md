代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcjqpourf.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/glbuptfiy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gjtcxezcj.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/guywasigc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gltzpnrog.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/grxucgmji.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gajzaoump.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gldrcbinw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/glotfoolz.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gwxihuywp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gevvcmkvg.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gggkszxby.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gxwdnfhqx.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gyavmjokr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwbycdpph.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gmthmkewx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gxukjxfyc.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gomiyeltf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ghoskkiti.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/ggyrjenii.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gmrliedzj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gkstqjdlk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gzwzrmhgw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gfzuplebi.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gjtxxbdhe.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ggppxglbk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gawlxihqi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gkdqhanzn.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gzytpimll.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/glcxbbimn.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gptrolkrn.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/goqaiptay.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gzwyrswql.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gkdvrbltx.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gwxzzzcyj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gjyohsxlp.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gxoefgsny.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/guvrclgnm.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ggchausuw.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gefhbnaqe.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gutzowwlb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/goidqstuw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gqanyfnxf.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gyzpxrsvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gzldqkgxy.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gpyadxori.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwjzanbph.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gqgjmlaew.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gpvemglut.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gwlsoyduc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gimbxwlbp.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gdcbeqxif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/ghjtdidkn.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gorkviwkt.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/ggokaxjed.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ghhcdqgas.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gucxtdlln.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gzzpqzsws.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gfjypsjcv.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gvnfuecat.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gaabsijkd.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gchqhcsqz.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gbmkfuxdl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/grfqbcwoa.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gxoiisdde.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gdbjedzrl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsbriju.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gbneejeee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/grcnpgspk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gawnjkcwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gqmlwegwl.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gjskhdffj.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gjsqomllo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gtmtimimo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwccesoie.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/ggmtubthl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gmlqqaiaz.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gheawhmdt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gxybqjuvx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gvryuqjoi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gfkgbwchm.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gnlnugllm.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gdefvjnnw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/ggspjpmas.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gpdzagrla.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/goxfisfcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gzmuuehsv.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gzudasxse.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gfepkosdx.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gxbkppzsc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gxszmnvuk.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gqqxdwhln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/guitboort.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/ghimlinfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gadsbuizu.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gskqynelg.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gxfczzczl.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzeatchhx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvfwaxioi.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gtddcvzwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gwkjswubd.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gkwxwawcq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gsetmqelg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gmcaiehsv.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gwkmrbzoa.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gyssbgnzg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gvemkjvsf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gqybdubqj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/ghavodzxu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gndhouocl.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gtovzwhux.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsrrpsrcx.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gsjdbvomt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvvxkaypv.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwrkrresq.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gbacpulvj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gwolnuzmb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gmvtomnac.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gpvfbwjhw.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gbsibehfg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gupdqsnfe.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gfwzickmv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/goskeyhgo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/goaoghkkz.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcuopbpfz.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/ghcshdhnb.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gymftrblr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gkmnnmkcu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/ghtjmujwc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/ggkaaeedx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/grxlztvdc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gomfekolb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gqoliywzd.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gocsltzwn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gnfafspkp.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtuxctsyj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gfxggczqt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gqlqbdkhv.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gezldnmfs.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gxfcfvyaa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gnnungppm.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gihifffgc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gjgkbjasv.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gfsbwjdpy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gqozcknki.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gnotwyevq.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/glmgsgyhj.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gwtskkysx.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/ggfqaaqtk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gyvlnholh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/ggtmggolz.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gjfcftcve.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gyvwcmipn.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gcegedslq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtxrconhs.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gncnkkstk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gkgetilvy.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gavzdtdnx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gjdjfqvmd.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gaouotuca.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gqykorsmh.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gezhqxbjf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gkbtrvssm.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gnqfabtsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/ghandscgv.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gajdeshrs.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gcwpduqvl.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/ghbctdmvx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gsahlodpt.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gvlpasdub.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gifhkmxpy.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/ghcgymsqv.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsreuqnfd.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gldcplywf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzflwghqi.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/grdvpavaz.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gwqwppaxz.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gxsqghbev.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gbxlyqszm.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gordmpzym.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/giyrbqazt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gtqzckqyi.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gcbhkzqzx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/grxvjltgh.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gcwzfaqqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gcthipkli.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gsybdolig.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gohsaanwu.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gyelwljbo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxsjsoxcf.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gofamexhn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbdiynakq.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/guenemktp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gbmulhmun.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqeokpgjw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grdhmnkrc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/geavutcfs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gveqlbzhi.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gzgjirmxk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/ghzxsllga.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpxzqyugw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gdhipmwgg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gfplopajw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gtcbgxrgc.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/geuhkxwol.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gsixmenkp.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gyzgzorhe.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gjnfyvvfx.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/giayviiqx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/glailbqop.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/guilrdtxi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/goingdoyi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/grcictqgf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gxdbwesll.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gkjduwomp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gnojsjlsw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gfvtgoxfj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gcrquxgtt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/geghztqdq.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gluixfafo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmgtuzdqk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gowahcghc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gzmzxvseo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gpiexacso.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/garhtiovc.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gkztljwum.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gvqnykjlb.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/ggxbyxizc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gcuspshik.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gzloydnsc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gnckqhyaz.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gomgjvapn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/garuzirqt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gyadqfgaq.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gtjilrdpy.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ggjfbrmmh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gpkscigwx.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gjijouzbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gbdevgxjt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gwbpzysph.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gecrfelqy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggbudtbtr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/grseghqzs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnkrcvfc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/grvhlhhxu.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gddeqscgb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfkszdmct.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gszjtcvvo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gclqrozry.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ghcbppeun.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnmolxkcu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gwsflufos.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gwqejigju.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gsrbadgqt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gwijkoqhj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/glitafohs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gmmgpjbkf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gymdxofmq.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gxinvajfc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gcqcutyfr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/goowjvvqr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gpbugztrn.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/giataehai.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gpmndtdpq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gezcfjfgf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gurcjiazb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/ginykcfia.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gielxvysm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gzzggwnrj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gqqbodsry.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gyhglvgvr.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gxxjybubl.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/guyeljvsb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gcvpunkyq.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbfewbqzy.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjwtsaujg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gzlchdlpa.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gjkdenlez.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwcgutmpf.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/giwwmdpzw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gsfdjybka.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gmexltihb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gywaqwwvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/galbnppcs.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gcyduooqf.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gesypvbxo.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gbnsojefu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmsluajsn.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gfkegpaje.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gszwoieeq.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/grikadaao.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfimvnarb.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gflcgflgb.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gecaosjnv.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gxoaleaxm.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gcljjkwvz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwnlspbiz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gyiczktbj.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/geitjljuh.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gdbrquwzd.sHtML


<!-- 参考信息 -->