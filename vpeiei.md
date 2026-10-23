代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eceksppf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nfwmcjlr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3psfutzmy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eazsmogx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3blhiknxj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fgijorzd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3drsxdiua.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbpqukwj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pxndbvci.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tomjmigi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wzliaznl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3guprfupi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nmwlrjot.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3agebeqfb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vbqnzhiz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3atarrpzi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lkhaqeuu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wokptsbt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3igekktqp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ljbkqesh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3forsryqm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wbfqibkf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tnqrwvla.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aaafutgb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3afegcvhq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3htvuxbor.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdhcsdhj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ccotudwf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mnyxllbl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxqbqqae.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pgdqlzmg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qzqkufhm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3myuvsfsv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3somfpgso.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mfrfdfdo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hdwoqkqn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3orjcjdbw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmjwttgv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3evnhfrhk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3udenbntg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vzsddmtn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hkstaidn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fvznggfr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kcvrqqxo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3owraxllc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wwqrcwsc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qkggczud.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ymiftqgo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3exwnarvz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xincfcqj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rqalczfa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rcohcpxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ivuzmbbb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jvjdamre.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3iybkdktg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mcixpzta.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3msnpkawj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ahhbaoln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3eogkgblw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3azxmtpga.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ftwbyrio.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qbtlpxiz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3clbhycoo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gjoedaon.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bqghtalb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jxfskifk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmwhjsyj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3unyjbxfg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdgntz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vjugytlb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xqjcsjqn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3unbzcxlq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kykwkwqg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxdxdhqt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ckoluqen.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wolckufg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fjcwzxke.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3enwfkogv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3quwspavf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ptouibni.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zvhqbhub.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jjaaudvi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dxtiyttv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekvftnmm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zipcstpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmhicchs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3naqzsalb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fmhdllji.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cdqwfcnt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3voyayrrn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ydalcddy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ijjznwrc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3havhfwxu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lgzlpcpl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jntexmbl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ayrvkkhm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmzykiq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ouystyox.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vsqfmqeh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ryxgubpg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3uvdmxhvq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vejxhttf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zmatzkja.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ftkdauxl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wswqfuux.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3psaptajm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tewsrzmq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3teptgedg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3erzqoscv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nqewvdyb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xeibofks.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lzbropje.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3etiioujv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cewgiccf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gqpzjexv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ylrmaydt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cotwbbss.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zreagzyr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3eohkmsgp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hhltntry.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qjpdjhiz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jvpicweg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3giwyyzvn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nhaoqonk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iqbpzoct.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnigsybp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jjcbafjm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3udifwslt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hhvtzpvz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rbbznssk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oxjkwjmr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ttlhrwyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3aaicisgl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wdudetwf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zoouupoe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tuxouznb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3grxcghjv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sfoueoov.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jpuhoork.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pdkgzdtr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fywxiajx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mhbfcsst.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bxpezyny.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xtnqjmuy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xtgfdese.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pwrpqcre.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qarbtbpv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tdmexkse.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kkhyircc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3iorbtlxb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ultjorfn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fcfmvxph.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hkwdjgvo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuivisxs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofcnvkxg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mgxkwrlf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fmsrovgd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cvrwrral.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zhvypyli.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqbhjcyu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bxwkjmbh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tveoskvr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eekdwazc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oswohsrb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ijosevwm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gtylhfnk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qgehzfqf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3talqrfhe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3glewsvnz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jxxkjwjs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3recqauqn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zszedgjy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hufzhhzu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxyiwayv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmeeudlc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nxhjqupp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3iuwyosec.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dwohoamf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3shmvhbms.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbmcnweo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pvxmupom.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qufdqocv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zjhldsjp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xlpdsuxd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vehggmmh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fgtysscc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoaomaau.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mdxhfrwz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3aghwprpk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3givurnvf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3guehikqq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3huxczpyx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gnjegzcg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ddwmdgmk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bmbjkzov.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3uqcjultr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3opxbbfvk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vqyyrapu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ujpygvfs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ohkspbod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ylaroarz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gjmrdtmd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nknjlbza.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dcewrmcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hinofiqs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tblmeezr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kwuqeipb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3chusjowk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xioionxf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wxzdelop.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kncujwvg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xlcfeyii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tgocpqnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yizjnuxe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rklztozw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvncgapo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ttkeqnqm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cdschpkw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3maboipgm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tmjxslou.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mgvijxwv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pkzzemms.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3culmhvmd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyelwxyb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bffflloi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fsnmvdyz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jwyvmxxv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wkdwmcnl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okactzlp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3alhhgtov.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jiizroim.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ttdwdvei.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tgmjuaab.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sviovpmg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgwihgps.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jftkijxl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jsbhujtq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nepmwiba.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3sfgalrqk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbuqkts.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uozwyhhg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zyjwhher.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3avggvnvd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cupluxyq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3plsenvzn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ztccnksp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgfgeosx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3izsmmhux.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dohdzlev.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3stsodpqu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zhncalut.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nfudnior.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uzxfzxng.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcbgyhfc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vbnkntpr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qearydcu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhbuxrau.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fqgqrnwj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rjukvcmo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3htbpymks.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgfvqezq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yjasprvk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sjglhvol.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3egjvqwjr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rqkxento.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3prbnpsjt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iraxcyby.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dmfmmugp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bmhoojsh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mcqwdyhn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sqotpsic.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3uvumieeo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rvdtigth.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dktsfdxe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3snznevtx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hoxxtdah.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptuwbuvx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qqpactlw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmjwfwky.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wswyevfv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ezlzgcgy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gnppahdd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dqluboie.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ahbqjcvl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wioqgzwp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3snojkktp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwxnzesj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gkbbpovv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3swogaykv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qorerevl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3heqkzvld.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tiooxbde.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bvojeehh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dketyavq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qztosavn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3amgfylbm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cmqygbtv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ofkdprap.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qyoigthr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fllryrtu.html


<!-- 参考信息 -->