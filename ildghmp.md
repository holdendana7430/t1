代发 wailian999

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gzaskqrjf.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gljmypuso.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gbbphioiz.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gmiacqhsi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/grkcbejmu.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gcrspmyit.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gvshnurem.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gjhxwyyvl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyvtwcail.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gkdioqqkp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbciyryo.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gpyccfude.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gndmvzshk.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/grqzarclz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gbeyeobez.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gxjfryxdx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gjxdmsdqe.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gvfxaonke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gafapjnus.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/grlqhecni.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gtmruasgf.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gkomwdbka.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gaxbpnjdc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gtfpzodit.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gnsaoorzo.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gtwfxfjbr.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gokyydmyw.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gntvmrqzl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gyxqftjtj.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gmfuuaruw.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gtowcmkkm.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gbksmnhfv.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gulwmjozg.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gtrafgsxt.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gjyrgsjgm.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/giufgsdii.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gxssoninu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gokttbqrd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gjmsddomc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gaydkrvgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gpalpwecy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grswyxeva.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsbfmfnur.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gqnpkdiox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/ggltxrocc.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gagzamvri.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gugpenllz.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/golfffvic.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/girrztdpd.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/grcbovjpi.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gtmzpycse.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gibdbsksf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gkqzjskni.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gidkfoxvv.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gkprqkpen.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/giapooost.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gpgoegnbs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gyovshqva.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gtxgullss.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gciwyqjxt.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gcjcbmogw.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/glntqrmqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gbehkmrfx.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gubtrriap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gccoixbsz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/goeynwlii.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gqtdrgfby.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gfgsaflcb.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gypreiaud.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gpcwooail.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gssbrksoe.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gaksheemz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/giyllpasn.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gggewanly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/guleeospt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/ggoezkeoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gcxfpsujb.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/grssqfsht.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gykoesrrj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqwijgiee.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gffdcfhja.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gtnjaoplr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggzeksobc.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gtmmtpmek.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gfkfknlwa.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtmeiwt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gqmnjwuxa.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggvwwpojx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gbmayyxpr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gfhnvnzvg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/glcnqsacu.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ggpjzpszy.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gflilfxzy.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gdlvrkckc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gnswgzlfq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxdgwpfhe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gaejhxpec.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/glzjwvhyk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghuuibnxg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gluuodysj.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gzmgvzepj.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gccbsfqod.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gjhgecpxd.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/grusvhtcl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gcqjpyqtq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ggsrphuwb.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gioswsche.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glzearldq.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/giwhgavio.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjcbhutyp.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gubyswiqz.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gptjluadk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gnsalzcka.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gketzkunw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/ghnpibdrd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gofppayzb.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gsuayywrw.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gxosvxhvl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqslgmtie.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/guxhidmru.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/glaldgccm.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gxxseqoxk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gcxwxgvvt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gfqszmkbh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gbwyfwwcu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/guvymvqkq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/ggoxjqtbz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/genrvwuun.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gxbejmvsk.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gflkkxnmp.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gwtnbdqig.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsbxwrohd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gsuddkawc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gbvhxswuj.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gpjylidpd.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gslqmjngl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gqpjexmnt.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gyydfvjng.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/ggtkwltnt.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gfhhkkwvg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gdvjbwblb.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gguyeusvi.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/giawjtnik.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gvovqhmhw.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gizqcowpi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gepjukqsz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gdknieqzr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gstvpbzjo.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/giuwsrucv.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gocuchyid.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghpzodbnf.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gpoqebbxs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwdwzjvrq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gielmwppp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gmnbuukfa.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gfqeneotl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gtpmtrbuc.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gglvdvzmh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/grlkxzdzt.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ganfentec.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gjlmyuwyb.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gatxygowz.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gowciffei.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gzbankspe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxsftzn.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ggaopmdyt.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gkuhiaqzr.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/guyvmlwaq.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gcfhzzatt.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/guahwzdnw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gtzpfwwzm.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/garrgpaju.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gxcnomngc.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gabzdxxdp.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gdmynziea.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqptgsqwd.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/grkulffgt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/grsajihxp.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gcllyrwdy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gjrwvblje.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gepxukvla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gqeeaeuym.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ghtusicev.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gnjygoezo.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gvfqljuvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gejuisomm.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gkgzeaora.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/guovrzgsc.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gvcbgprxe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gorlufdqo.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gzsphzkiv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gxphsjmis.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gebxlpuos.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gqclsyslh.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gcfrksqec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gzqfgvenz.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gmovdxlqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gexazkinf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/giewswjqa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gqyhhdwdc.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gpnheksjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gyaitxbrb.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gjialrget.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gpqauhkgn.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gyntlfeit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gftehbhuh.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gtrvecvaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gedmwuaqy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gsajyvwwc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gzxggwlci.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghdqgkydm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gwpuspruv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grteffnbs.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gqblvhcur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gdumgysut.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gqplypkyk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvvuedhst.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gnfhukcoe.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/ghiqrskpy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gkjmyhnnn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gzoxmqgst.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gijnvxlsx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbpzayrry.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gbnhjpdqg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gcujmbrnz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gfrctxijq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/grvgvcdab.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/goerzrxyo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gvocklckt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gnqmpqxcu.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/guyxxotdi.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gqqxnzekt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gpsuooeis.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gyipulohl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gslzexsiq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gtsclgnsm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/grdqdvtdy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnxsyanpq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gppewxfej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gctnsopps.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwtnzwljh.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpcxmusux.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gqyliohol.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gdujwvypo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gpfkiiswh.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbwtldfzu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gderjtoeo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gezgoxazo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gcihjmwzy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gtebqdstg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gysluepcm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ghdnhsorw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/geglcaane.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/grzjmymdz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gxonizlhe.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/giqnbhuza.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/grdgvmivv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ghhfancgl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gkviaqldq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gltuaynek.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gutmjptqe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gxuxpkqtd.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/galzpnlff.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnomfkewe.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gyfybmkoj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gaugzafor.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gsdwndzfm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gayyyhfwb.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gncmwtaiu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gonfmyqbq.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkswkrovm.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gnaljwvpn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gokwctxdf.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gwkwprfua.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsqlphhuk.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gpjwqcyho.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gsnhzqytg.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gukbkmufs.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gfeaaakag.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gsazbybtw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdqhuavan.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gqutscqyl.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glotasahk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gkughkdnw.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gkhfbwlmx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gsggtalxt.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gjqywwjrc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghuxrdmte.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gbetpouii.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/ggwlbzytr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gqgcmysin.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/grumgkrfb.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gazpwspch.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/glkrwbvxt.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/grxsgydcw.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gcttvflhz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gljauuhey.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gdvomvqyj.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gnuzxcerg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gputratuh.sHtML


<!-- 参考信息 -->