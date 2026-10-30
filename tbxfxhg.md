代发 wailian999

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpazjymn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/glqkberkk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grgfoohfo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxsbvgmt.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvvwenmp.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtprzdsbb.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqjzsgx.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gcppqixwt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgnnorpr.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcodvkwq.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guyopeawd.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghlfcqwci.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnlsbcnlw.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtgcdbks.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsunztdpy.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gisaqvtky.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gwezqggif.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaegfwon.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwifunq.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmyycaf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfafbrfj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihpiazwy.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazcyqjm.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbasflm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqumeujo.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtberlls.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvuikzoal.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gorqchnzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydrojoj.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiletwkt.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxivltetx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjghbbde.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/giydxiyho.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggoaewzfx.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjwxzvqn.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gyygwkgwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gpmgulzat.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxuqukvr.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gowszmufu.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gilpwijqm.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzmvxxar.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gscuoaekr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gapmfgtca.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcerbzuuz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/giccbnudf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrljjfor.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/goajetwdv.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/grrhqaqwm.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/govybjdnr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gduvqgdcj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpodbbfuk.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhtyjudx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gfncwratd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvlhwzqwv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggvzdgzgm.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gugxoowyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhsatqqe.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggrghrnzi.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gczftgebq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gpsczhgmx.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvwentrl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyzbwtcc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzluysqgh.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/glcktjexg.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnnqxqhn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgbtcyty.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/goomwqvra.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsveqskhc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxkuiaap.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gqkwynvat.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmlpmgkbw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpibodxh.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gtiigiihg.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gglmifirh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbnzjgqvk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyxsconp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gkyolkjsd.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkddqsvzu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guevekazy.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ghjlpicno.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkkptlzj.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gargxywif.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghmgdynpt.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gbquebkcq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdjjwucgp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimqtrona.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyxjekkl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxdimzwwe.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ggueekzlf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gumfztqwr.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gllusqrwe.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpnnphwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzmuuwkw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvvfvzpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimdznhk.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjcktlnxr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gobbmphka.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/geqcmulor.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxliyocr.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/giphrocqu.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gotpqzywq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhmpygkr.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhlrlzzm.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkaewcgnc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzljkeo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gbjwazdtv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmxztrvi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluthmssw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlzigah.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtnuiyma.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gciykusgb.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkyommopb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwracyqkp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gypmsqtvl.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjwyayjza.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdzrhqkk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/giojfhpum.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmgvlfrs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvezuhic.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgezdjjw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/ghwelcgdj.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggpszpacf.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdmidsnt.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gglgbwjmr.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvskmqav.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyzzfyphq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxnqywfw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchtmtxh.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gjucervot.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbffymsbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhwjhfm.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gajqpchkn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gqjnedlbm.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/graqozukr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqfkigdp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcuaqbgr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gctepvjhi.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrtrcud.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkedcwcij.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpnxzblnb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvgymdci.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gasqkucqf.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzklmbvw.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbbfnjuu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzjqwvrg.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqoznvv.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzresney.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gavxzmwyh.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchpbfcbl.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyuvlhjw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcybhsrsi.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/giowdnezl.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoszuhvb.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfmhwmss.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndrsqowh.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gegipbeam.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmhezyd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcemdkpmn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqexixsv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gmilwktmu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfqgelt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbgikkon.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/growlltpq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzrvvnfe.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtrjmdrml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjypiykhu.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gllunzfhm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnjjujgzm.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/goxsgappx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grwtyuchn.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghiprjehz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gammbzicp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvurpluvm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gionabfwm.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmxxbuprp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhecuwku.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcepdtnoy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvruywapu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgxcecd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/geppaeduo.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrskelma.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gljfmciye.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqxwftcw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmakwwdv.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gghoykcmx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/geujtdvpr.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoqfbazt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyfjjtnj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsidyvql.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmtjjljpk.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbfmhkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gazmclvnj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuphqtnb.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjolkohgs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gckzjrjsk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxddckanl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhetoiqe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gumawmlzk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuitzvrt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/ghfdtoyfq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesxbxwxz.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gfzahsxuu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyequdox.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxqjqngy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/giqxbqjvn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gvwnvxkcp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganhhwaxh.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcuossfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjzpjvvqj.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gcchjvttr.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrdahejt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjigqqhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gujszotyf.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/ghymzjtlm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gqapbcgbe.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gtxypntel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gorzhyzsb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjhyermhh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzbggiix.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvhfpjzj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gozwdehqc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnxttpje.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejwgczc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gamdvhibg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gptxhskmh.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnrcdacf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gdibskxke.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdayaae.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmarevvia.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsgkpfha.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdyrseub.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluetpptu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gqujliknh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcybocbx.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gqnghkxxs.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqubdrbyf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxurgdkoh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegcjtho.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzqgnwfab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gurtuwksr.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyyykvdu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnqjzbwx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmqkitp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhmjphz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gxsyvdewe.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqamyfjmg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsrounlm.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gheirmxed.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gdknaubsu.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzalycjgy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssrxkmxo.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gioyqhaqa.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gjzeenttj.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkysxjeq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxxoihnm.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjqnials.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbczcut.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhhubpos.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gashdioqp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmmdhukj.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gifvdwlwz.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwupmzo.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grumkkqcu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvpsdaws.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbxnhlcsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagjjhusd.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gwrtysoar.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzhrgooi.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gttsnzuvq.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiarsywg.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyalptew.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypfqjjmc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaaxkflg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvpstwur.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gimvaipxg.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gajthibkh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gszefmsml.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gcthtastm.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/grbarelfe.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafcivbbz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghafsoml.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/garnatnnz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcseemyw.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzikmaelk.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpocbspih.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkdkybl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjhkqal.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfvmyroe.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcolwbcpo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gojkmuxma.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhkqmnue.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gagtidkyu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmejbode.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvnlnzjj.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvjbwxbx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxgphill.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gvlfsimrh.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgmlloil.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnbpynag.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ggqcypkjl.sHtML


<!-- 参考信息 -->