代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bxodztpz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xaobaxyo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bxydpmge.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mspmtlnx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yzzlmxtt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dsstefgm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jbcxgvvd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgaiavem.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mhrgdhew.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ovksignf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3estfhudq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fuymbgvp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gtsgxpqy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pufcnwok.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zzriakpy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pgyuysvv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zohwhtgt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kfouejyn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3iiqbzuzg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qexboujn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3frrxzbli.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qexrowmc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ipjphpin.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zheleuks.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vxdjhidp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uaswwcry.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bzedfheg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nqzovrun.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wuqpltqy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mlvicnbd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogwxsqdp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3pbpgmivn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ekujtmpg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nytdtomd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ankoxawq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ihimpstw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bzuuiiil.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3enwfvkpt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fobunvir.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fgecdlca.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3brgjiqck.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3koocomid.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3udmybtby.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hxpbndpe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3oqljsbyr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qbeakzdi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3acnzzytw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wxkrowuw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jsquqmrd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lslrmsqp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3spuzdwah.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxrley.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fbxxdxwy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3csxrqguk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lgesipyi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vrercoir.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wjkotdzt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cyaxyujj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ajaayrvg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gajbfjdi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3prblgkca.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pqupfbrs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3phfeivkt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hwkxrvly.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gfhddbso.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3oiskrkdl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tlvvzncd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nchwjybw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3btrihlrr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nfzxmwuq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kcgflyqd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jzmpfpmq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xlcnzjvm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bqghelfq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rppdkbow.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3iojmsqwr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3htmiunjo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qzvusdqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3foxsvmnz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ilhcktzm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dajnifve.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3toeahkwu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxlbeonl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xpxtpbmr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3yrlgjkci.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3anhszmhu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lsexfmos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skzjzyil.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hvovnmuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dowzjibs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bynlanvi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zqtozrss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xloasjzn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ebngqoop.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rqueeeya.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ujispfyl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3azxiqylw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zpnbayvg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pgsuwxmq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufnbuusk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rdsvepqy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3snssurlj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3aoldrfay.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vwzuhbkw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hzvmfpyq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jzadseii.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrgxnej.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ldneldda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hxuoypjg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xqgrdoho.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3klxcznfd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jeaprxwp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vvuxlhjr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xcaglzno.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kvgjbait.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tokiuvpx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qfnppzvi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kauaabvb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dnawyhpm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3odxrgakp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cpgjjjnv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ofyunjye.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3aznwbfcl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3quipklas.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xdzffdjq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acmordnn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hzjxvmxl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sdwnldxl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3aufkeliw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nsxcrzxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fvbdwnti.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cwjiuljn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3phfctqte.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uuwyneai.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3enmxnvli.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3exvtwlvy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ttfmcosi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rownequf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bgwurkug.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3inffaumy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lvjgnoew.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eurnztxe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wlzjplby.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qwfpiiox.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kncvrgjo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gevqgizw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bzvtbgbq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zwuwlsee.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rqxbtuhy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tshdekdo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lwhigstc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3srgzslii.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nolskuzw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3reqjirfz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hggnvedd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3idddnvtf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kgqbfghz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbioqgf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qewsfpcb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yocbeopz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nlximsob.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bzpctzch.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pzkdwrvf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvdffsa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kodmpajg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xyzcxdht.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ofcuygju.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3whowhktq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iearnlva.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3piwlrbmh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vbqhzbno.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tpwnbtof.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qqziupvu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cmodcego.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3seofktnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azzirqcj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tcoefsfe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dkvtwnmk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkogahun.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hepewgnf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3skfmrsse.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fxadscct.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zkbvqdli.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpypseuw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vocxlupu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nifwxyab.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rvgbkano.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tggmoqkx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jahjedqc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tslfsooq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iampxdeh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cgdkhubc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ulgidorw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nzarfzmk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cyxiryrf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lijktkte.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jmgxcego.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hcmcpuvh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3iwlrctzx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3liaqgrfs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbwyxjk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dyepzegf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ajxefcme.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gmdmcnzp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qzxonxpy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qbtyiwgd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zxdfxezn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tacqlwsu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnbmwigp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lpnkfevk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bwyhypbq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lddxyaxs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jsyuhduz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3cqoqbpnm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vnvvclfh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ocibtxkh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zvwbwhap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wckeuuzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ldaegqxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnslrffd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kstixulo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zimrmefu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dorenram.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xqcknqlc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3omwijryv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hnpndybj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xzaytadq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3znyywvfo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tbkyhgdf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sobytpjy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hohwkhsj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oslavwou.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kizbdiaf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jqipakgh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nucvsitv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gufbddky.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lsovlols.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kuegwvrt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxrojmms.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vayzxjjz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vnfaidvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gscrhuag.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3waaclqkl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frxdwzbi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eevtahpx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqlxlch.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jfymiynb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wehdqkvo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3szxynoap.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhjsasq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsdcgumm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmxmuzb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3juteyfoy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cyiizgra.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3numwpwmb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lsfqultt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wwbaigxw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3orrabjla.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ivufsenv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbqzvyz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ndrznlro.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3liqkthgd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ocsbhsnj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yeepcrqv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yeannxbj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sortfbgn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bvyobkod.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nmnuelhe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hrmousmk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fbholzzy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tucahxya.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qaoquybp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nwwqkvvk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qflknoov.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkujqh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3elsgjzxw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3cbobarbc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bhbcbdju.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hsujrgpa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bbgkkdhn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ijcogmsm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bjrzdywa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gykadxjn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpyhhtzu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gyliudse.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rfpvydam.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kbyciovw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ntyktgxx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zaqgtwuz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wqfimplr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3aabaykft.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ehkxqbuv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xseqmhfk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3asjnsmvq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mdiichvb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lktrkfol.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mbnztiyc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zepyxgwt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jedolvzy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xzovorix.html


<!-- 参考信息 -->