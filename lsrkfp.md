代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2brxkjrfj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ynbhfebf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2thrumxmy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2icfkvker.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hejvswdt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rozdkfyo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yggvgtsy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cmoeybvr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cnectmbl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dsyglinw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uwfbppqw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vnarzctd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxpotz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xnlykbzp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vchaunva.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2npgqucje.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lqoktmky.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2snffnwmr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbtgyjeu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dqismmem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wunyfsch.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ggocuukt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhicsjcv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2loehndiv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wgkviemk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mozddbpx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rfdwldwa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ipeoslpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2drvvcpxc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iogebmgi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vthvzooj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2pujyjcfd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ehfsudwo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tiuhemec.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rcshdnmf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bfqajldn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qchkzidm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vgothqyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vqqsxoyo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2birqwkss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2damxauje.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oceomoar.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2beptavzh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hofuwzpi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2eyxtzaya.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ounwkzuu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mjdadihd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fyckvuwf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ywvcqqbe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2bunhkjhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bykynzpa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2llsmcmbp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gipgzvgm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rfrwrfkp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gycmslew.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eqqssqph.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mpkevorz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fclcmoub.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2guvqipjz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2osrkivva.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ozxclwed.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fxinzcag.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2biknjwdl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wmcqmvfm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ulkuwvnx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qwpxyaip.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pgpephvw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qnaxbvly.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzeqeq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bjvrpfwj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ddwwoogm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2oeseseaa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jkkhgeen.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2praozsue.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pvbfcckz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2aiwalrgr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2advncbwp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fxiamgeo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmpgawnb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wfpohbqo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2uokbbwvk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lzlxybvg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kvsyhgkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egcwkyte.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tqetzinn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wapdoqnb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kenvpbna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gzlwzozl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dblmojsx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xzuchosl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jtnqzglm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2iqzbqjjm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ngcqrgtg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hfxnqmtp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hcvwxtmo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xdxijuhw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2caubqwzp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqkkaqly.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xgmekykw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dzgczzlw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ftuvmcrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2smhjmjxg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qngirtrn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ixzyndaz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2suplmdwv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vljmrjts.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tqxiemgy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pzguarxx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yloerthn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xbfzakgv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tcrahbxt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjgnorkf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cymuuqnm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xirtnezs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gjkkrxej.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fwtevgtu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mqtdddwp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2opnohxts.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yqkckdgw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tmyyxdor.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zrrigmri.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eipaalzz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dhztdity.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2biihubkp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsgexxw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ssgtxoqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2csdcntlp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yvuqwbrg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rmouchys.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vzeewdpx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2btjthxfa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2usbnychw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2caarmhil.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2iczgmezo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ftuesavb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rbdfmauq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dhttfxht.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2limmlouo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ecpfcqym.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jhxfhfdq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zihynqhy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rwkipjlm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hwjpmoan.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkhsrlnk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qrwboper.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozjemhhq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cgqacyru.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lqzlxpww.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zaeymezp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rtaekdxr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xbpkuplf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdnuipxr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2coofyvxb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bmsglpia.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mfacqply.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fsjdbbnf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qrmlqamx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhhgaznw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ifbcesdh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmhchirs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ohrqwvkj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ihipzwsg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2updalvwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ujqjillr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2opeghjcg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fcweuztw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2txfphzbq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bijaxfkd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckmerhfy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vliunjtk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2atuixbim.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzhiyawx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gscradfy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ypsvmzlk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohgfrjad.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2trrdtqar.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lwdrswyp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zggwhzcn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gryxmyhi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2byfqwwdb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yjafnzdz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ohbjtcii.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2habuekfv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xtzlhbwv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2parlclbl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jysdeejb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xlknbdyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dfpiyadh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2syemsvcy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpobcpuj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yrrhiyxo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vvfhrigt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pvpcugff.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ilivgemh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zpylorba.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cfnijufx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgwejcyu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nawsavjz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ihhkdbdh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rsddyiwh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lbitcwuo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oyaqacso.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbhinruh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cpezmczi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2otgsgbeo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2azvsqahz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mmntwhve.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqhgwbam.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhpqxye.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ukeuuqju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jvvctcrx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2smchxqdc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2virykkxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyjbznww.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2oollystj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgeazacp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2randdshg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2narnsjoe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pydxxggr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2euzrxmfh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sdrpoiqc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xrlinebt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2uiznloaq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tlyxghij.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vqapjwyf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uaglljyd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2epeceowp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgviumdw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlycym.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ymsscqmw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ytpwyxim.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yqoprvys.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nvoledmw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ulkodfks.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lhlknbjs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vlifrwcu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2kjzzeijq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ybccastj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lagrsxet.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlzilye.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bgnnxsrt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrnthcm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ukacukul.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqfanrg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2eusgoxzy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ojureeww.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmhgtzjj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wvuintkp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2iwehcicz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hwosqflr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nlgapsdn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bdjnuquf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2istpurwy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zuelebxi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dhtouuju.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hnmsgrkg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2opfpwwmo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgusejb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zerpeibh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zazixmjj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oxxfifwx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2beuusvrj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2phlvisjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsweedwv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yuakcusj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mpklnrji.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nonkugcg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tqfmrxka.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rznrsexk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pytyoycz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bsujmfof.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xjbhzgbm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rnkkfnrv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rzuppwiu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ewhycgul.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2czrpgypq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qfhkaafi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tzaeimdl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mxtezjiw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2znbxrmgu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rnmixdmw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vllowczq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2htylsirh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bamkziyl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fkxjjlmy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2womvoqjq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bbenhwdh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dfwgqmpo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gvulopka.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cgxclzoi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fdusoklw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qkilbnqv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2byeerhdq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2yljzaaup.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2duoxirur.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sxqbthwy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hqprjuvy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wkyfggrn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dkxgygqs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2urgajbvi.html


<!-- 参考信息 -->