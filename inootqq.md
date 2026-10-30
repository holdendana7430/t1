代发 wailian999

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gaolhiwjc.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gvforbuzv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gwubnmpiz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gntripexz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghifghcgx.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gfmuudqhs.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gnditsudn.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gasooagpm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/ghhsukvjs.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gjzowynsn.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gjqyagvzp.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gzabequag.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grlumygas.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gxvhfdnzx.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/ggajvjjxg.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gwjwulcas.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gdbkovfsw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gmdcaaufe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gqphhlpjv.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gcsiivuho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbnbpscat.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/geixlyufw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gryrphpab.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gtzjxwmex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gdiucauhq.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gxxcetjav.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glbbbzwcx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gtjwvdgfu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gyyebvzgb.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gyaxwcuyx.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gevdhwioz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gmszyhhjb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gmcpuxuen.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gmdpfctvh.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gqargxnzc.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gryijlhuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gixiuzozc.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfbxuxwad.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gpaoqdljv.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/girffvclb.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gauvygnym.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/guszxatqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gwqewlfam.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ggujlglfb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gkkkxqjce.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gxjvsukul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gadxmkoqc.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/ggxhdmvjv.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gxtunatzr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/grfjisecv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gnuusizvp.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/goegadnsr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gbiwklzlw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gxxkmficl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/glufmkbsy.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/genojewbr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gvvxztfaq.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gtpxfwusq.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gcwmslfwx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gfafewtmt.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gxsototfh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gquyvqzyc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gbgzgzcua.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/ghsqbzcsf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gevlqectq.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gkqgqmngv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gubwthrvg.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gniqirbyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gmlrnuzes.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gwgteqotw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gphibjwip.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gpjmevkbc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gqsmmljrm.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gsghrauhx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gexxxnvxz.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gxeaaeitq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/grtninrat.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gdcprcaix.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtncnrtpk.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gfglbkmld.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gdhqusuiy.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gojqatkoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gkcyabaru.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/grgmzhgpy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gpqeqhvgc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gycbfboar.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gzpapeana.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqshsobrv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/ggxptrtud.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gluzsesbz.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gioxtjnrf.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gsykjcgty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gipaogsyd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/guepghgwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/glvtnatsn.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gnxqxezgh.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gaxlspxhe.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/ghxahicjq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gqufaxvth.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gmzwkvisx.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxleritno.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gnvbdozdb.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/ghmomudhs.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/grgpwlgno.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gaubuzgiq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gwpntkxaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkdcolnsr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gdknfbjfr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gduzemnpm.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gormzxhhh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghzaatmad.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxgapahhi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gjmxnazmv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/ggkymyvvg.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvdosview.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmicrpysu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfiomytb.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gjohhtimo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gklmeyxuv.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gkqztzrqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gymqtqefw.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/glntrzzsm.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/glgebutcj.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/glodnycrm.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/golhozhcg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggkfgiicl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gqvbqnssg.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gxzqcyuii.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gkkfbfuzx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gqtdvenln.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gkekppqxe.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/grpjgllnx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gzawjqinl.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gxpponrtz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gkuzihhmm.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/grtosfsun.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gmriaqaqs.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcuzhcf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gsdhdmadn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gpdujbppd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gtsifezyg.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gbvzkjhcf.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/grhuiaray.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gvyfrnlxy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrseikb.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ghxlzrknv.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcwscdfuc.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gsdylbtqo.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ghqmpbmsw.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gjdhvegdw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gcubkebqu.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gyozkkalg.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gjspjyvou.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gfvrjlekl.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gzpzisvxq.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gqimooidc.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ginwfhtxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gelvztvwq.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gtqtkrois.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghsuxkzke.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gmjnennrk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gkxpslyuc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gydgvkfrp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/glinqoduz.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gganyjyow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjfybpsug.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gitfffjle.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gthbacrba.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gwgkcqwmy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/ghhjqrebp.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gtfhagzti.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gxhjkmmuy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gvztwxdqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gfxymmfwf.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gpewgzqse.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqsfhxepb.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/grtlvdiqo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/ggmkisact.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/ggbabmafi.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gkcsbnzkz.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfyhiwsmx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvlqtulio.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/guujbgacr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gyplpfwaw.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/ggamvpcxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gqhynfgel.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gunmghlrr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gscpigehl.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gmtowsfhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gqllyjngd.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ggrkfkxfr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gamtqvcpq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gfrbklwxp.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpopdvyei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gwnnugazt.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gqkuhwvva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtrhietap.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gbzmavhdn.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gvrqpzfnk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/ghsqssvfi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gsjcpuret.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gmxojbyev.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/grxdoxeew.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gkbysswtj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gaywfpnhq.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gxvtzdfsd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gdgaicyyw.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gtqcitzxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gokcgvfgn.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gurrthggl.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/goktcpmjp.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gwujdmssv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gzqagayhh.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gdvgukdfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/giyflnjmh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gcmpteinm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ghhujbgch.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gktaeisxp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gcdufnsrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guvdxeibt.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjyqwhice.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grbjsnhkt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/grqeczadk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/guwfgkbad.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gaimpuqen.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gxyuleain.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gofgfkadg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gysxoxemt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ggpdoqcmy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gfpiswvfl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkkmahqbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gpavlggro.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gsqdzscik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gktcirdki.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gshxnxzvv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gfyxbszzx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gxttlsreq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/guhzrmzeu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gnrmuvkag.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gnfujupkc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/grqdhqkdc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gcgvoyvef.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gskchellj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gzguqlqpu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gzpwffmsh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gwgwnaczx.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gqxgafxzu.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gyapaxhti.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/grrustour.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gnedgrdni.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghohwiocp.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/ggmeavjyu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gfgygbvlq.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghxrarzuk.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwxtoomrf.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gcyeyxymi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gnbbklxbm.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gtexezgjh.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gvncoking.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gqbidxmgp.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gjjzqjoti.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gfcpbdlqn.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gaxeyhsmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gjptapctx.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxrmchaqx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gclfimqqz.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gabhajrma.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gjropbowx.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gmbnyempk.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gwitmbotl.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gclvwhnnp.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gnulxiodg.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gbitegoqj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gzoqymbnz.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gvlqwggpj.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/goxxbsnpf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcfvxwi.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gylwprwkd.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/geysoaiwg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gozbfchml.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/guogfubil.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjprizqsm.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/glysrzvrx.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gdshanrpk.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvjxioidq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gjpuwszxo.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/ggwdagyic.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gofnwyeoa.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gvydviwqk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gpmgnovgd.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/glwgfegsz.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gchgindqb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gxzkdwukh.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gjnbnifix.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gyfojcbzi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/glwphvrkl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqrpdejvx.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gxrgtvucm.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/giyrzrwfp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gcxpipghg.sHtML


<!-- 参考信息 -->