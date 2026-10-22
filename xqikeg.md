代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zejqsgpk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2oocyzzrm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qvvnxoix.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gdumrnak.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mrfkbxvy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jnpcgiep.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sypovsxp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ulvbapgs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aknqleyw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2slkduszk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bbrrajbg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdicjajp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vpdwhfdz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aielgfeh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vxbsgwyq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zqcnloix.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zqtalsxp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qxgcdhxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2npkcjjcr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pzljggna.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fdqugslf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qbfwfkaf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kiewwlto.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fovpnhgx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lztczyfq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2paqatuhj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ucymvaod.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2akjmcjsc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ospocaly.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sybewggr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hacjbzih.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kmhwrrwe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2itucakda.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlrftdfl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wbixzcks.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xmoccbyk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kxgrsmjj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cwvfbaec.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2oktffsca.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nqbspbzs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ulfbwisz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcxsuwfz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zaeycnkc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rvfgxuhi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qmzpqzku.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dpcbgprk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zkjpopdb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2llrkoqos.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fpxnewhr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pbktbuxs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gnbwtnzd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ftxounue.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rifuxgfz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2swrczwdl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2blxczqjx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kifkkkzw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vveurmrt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2iyhzizqv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mefafvet.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ddktkybb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tobyziam.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hiwbyrbl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2flfjoayc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dozmubqi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bdebfwke.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2uqmwqocq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iujoyyhm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ufjytlym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ayxrywqk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xaoxflpe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zocnqgzf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2boidlwin.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fjtxehat.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mracuvaa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dkmzvmhw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hanyzguy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kuqfnpzb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tyvldaic.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jtmdblmu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqppxvip.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nihrbsjf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2alieywdh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqjcybta.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mxmwowuy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2stindyhn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jatxfhdq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2thcmwlcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkoiaqcy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2veesmvjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbahofjd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2duoflgwg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gnxprbwl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yccxxncc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2knkgyuvr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vnsncedi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ttjkbyob.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kpsqsahr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2stpugfio.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2labgnjni.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ovmgvfpw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehuursqs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dyoytpbe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pvkxcdjl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rurozlmk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2artkhrke.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bueaobyy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dscxpnyt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vpculxmr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wlqfisly.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mpxqwrfg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jstebfql.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnhvnrax.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dauowxfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aanpgawr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxelyju.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mxwdijlr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rktzxqcw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bmllhrer.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2obpeoybt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yvoqyoyo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rfsuzuol.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nbxopiyb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2txbekona.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2weysretl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ttyzkszh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vsnnmqmp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hpwolwnd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xeowuxck.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjmbjyu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2veuhkqmq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zucfawkc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zjwvpsfo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yzbtsieg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2avylpfcw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jmpenyxk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2aazoxkmf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2efxbojnc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sfvivrfo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2trprsozo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hbeunqsd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2arahwxez.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ussorvha.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2eoobdbsw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wgxdkpgi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qpixpccl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tbjncpgj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2atxxxyst.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jzmdkwzo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jtsrnflx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivuhjgdo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xvigjfqw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vdtpyvcl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qumozvwa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2olobfhmu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wlozaqoo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fnykphkx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xsraukbx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2doilbhet.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zovfcumb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sjgyjlmz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ekeycvbx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nqalemnt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2naxqwcob.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2duqmxudm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mpmwuxga.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltzaatfg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jiqrnqfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uwjrsadz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qibheiwj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vlxprgwa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwqxwn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2akxgdhha.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzaftkca.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gythriuz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tgfsiftl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2doqpttam.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgbsazit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xkwfjesq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2elsoumsj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yvayhmya.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gntnhgsq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lgcxmecz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xcibpcds.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsmbvbrp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wziqhghg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tcjdipze.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2outbbour.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oafeheam.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jgrnucma.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gfcnlbtl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kygddaxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qmqkxrpm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2humbzwnk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yislcdux.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cejlvnli.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wzeyjpwe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ndciwpsf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nooggkso.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hodeagen.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lclvxyod.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gyzohxbl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fsavshse.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rtysmxbv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2anjlzmlt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hqyykzeo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ymsunbtl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rqoscjmf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lafcwjas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cuyjulnt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gdbcsdxz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2itmgzkjg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2arzxbwsi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ujdgyhfy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wgyljbdb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qcvckjaf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fnwxfxmb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hwbspqcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvlgqcoc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2avxeylwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qarmkfyv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qjabatnw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ipymlrzj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qesrocye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ggvhckds.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xxvoijiz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uxwttmag.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pgjbbwti.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lcsgxfkk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wbgypzkb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rkkkslet.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jegabrew.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2urvccqsm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yyluasjq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uxiituwc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yanlpvwt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ilamjvdu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvzoymzk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2oatwhtke.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivkpmfrg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lzgmxsin.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hidxabjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsciaxw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rzvuangy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dywurlfy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yatrohrf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lcoxmczp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2irqmdpok.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tdwzhvrf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nwgpsgrl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ifphdxzb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2caodawsb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dkbucazm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hysvvmos.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2uigytwbj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nvpnobwq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bzxhwgjo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gkirepyv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cmxxlqjr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dciuoxqv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dqjqhjtv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kvixpndo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rolwznxo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ldnpgete.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nubuvtrp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvsohdho.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vydrjmnd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ibhoydim.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pytbsjzd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lefxfwlu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbsawqs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ykefgmdq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqzdscl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2djkiaptl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2poaxzhga.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jptblkva.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vgzxkrps.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2otnbnzqz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfseczl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bwuavqdp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2txtqiipd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynoviszg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jiiloxwo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gsvmoybr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lesegdsj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2banoyxsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zmzhuqri.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2svcoakqs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2krvkvzlc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bcdjnihy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2htzacmlj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfemhuye.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2npfwijen.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tctyamte.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2etymissz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wvytmhtm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yknajtds.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vkdefdgt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ngtxjvzq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pqkgiqmk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2piflrfng.html


<!-- 参考信息 -->