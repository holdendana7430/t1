代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3scimxuff.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3otsyhlpc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qxmsttnz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fplcbaxm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kucrkyce.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3noodwukq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpykynod.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fnssehkp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tfjevulb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tuvooevi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wjgioecc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3sxfjmedi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3htfmqyfz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ntormehj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zjfdcfgo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xsmdvpyl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovlsaxyx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tkwarlrf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gdpctypj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tbcmvodh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3msbgpyqz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wswloysr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pozscfsv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ddddrdhc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zgfbzovb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pcenkgmm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3slpwhbgn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bixurreo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eawknkus.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jejefvig.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fokgquxa.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mzctohrt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ahxgmaei.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pixrtnkc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mhwmccio.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fcrqouly.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kfagsqwm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fuowneyc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3opahiufu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nebfsdwt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ewujmfdh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vdrlzyrp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rjtclycc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ncjetxgc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nbkspqbv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3smzuywfq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rbjbzwfk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cndxtgen.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pezolfop.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oapnygvb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3owoiprax.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3whfbrdaw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3etorovru.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3oymvfnda.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kqjcjfds.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tuzxdihb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bhzjfdkq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fcbvfdxs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwcsnzkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ssbxhkxx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ewdqacww.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qyxtoske.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wfzmhyrt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmwlrnrn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3khxsmriz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mzffmpvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qhbrfnie.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ulcvkjgk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hjkxadtk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tueedyqi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3csdaxkns.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xawmvvxe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sgmkngmp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gyvepxqk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lnrnhrba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nmannrvc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kfvubqxe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ynajoakm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vageuecz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ujiaxjfp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xjtjjkns.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qsgwlzqp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3futcvtzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfhkut.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gaekrfau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grhlxvho.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orzbnsux.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nhaunvhd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdoxeh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ezdbsqub.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kkcafqfw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vpbvoucw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3oewiyiwy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3seusarnc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gyygzhba.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nxlqando.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfmjypfl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rjaguiwq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ozagsmzv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nziooxeh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kqmhctea.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ljrbgobi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3byyqxdpk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3visluohl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wunommqi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eeyopesf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vqhjszky.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcgbwplb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3onzctfyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ekiulxju.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jqhifiba.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffpkioot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mfhqpwae.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ipctgqdl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ggegdpiu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tpqjcgbo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ekzwsmwm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dmksazqz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qiuejoeu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ghsrwvpl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kinfmxfx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vkxuwzuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vpitoxsx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nuucszsb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3edrwrzrm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jyteuvlv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iyqvyeqg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iwnkiyzy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ffmmevhk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhjrtbei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bvlkihbt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mtqwkjhb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3apjvkqeo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3azlxxxpl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ggakdqbc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3viiijiob.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3iohpuxmm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zbfhgwsu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ordjdrlx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zjfekjgr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hotjhngt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kwsswiap.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfcjzqpp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mxxwjraw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gitohvzo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3krdbxuez.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qemrjdln.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3htjybeej.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3irdxkvzy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jtawcaod.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bnwxvfda.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vnlnnjix.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mhoovstr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rpwxprkg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cyhmycfb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gicnwuso.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3oxmlbrkx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lbvqcfts.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mnhcdxup.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzeifryk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jahblllr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lzehqbyk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pdruseyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3umnmesyu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ojrszukc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vruehdbr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ghkgvwhe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gliaboyq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xooefdad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mvogdybd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hvfrmckw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohlzpxix.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofnyrkng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qpgipqlz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oxvevion.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pooqxcoz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3sjhnooup.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zlucuqkc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fyfierbw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nspulcky.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tejgstwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yaitywsg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nwpgkhgv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cqroidwo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kmuhyauo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bqdpbdza.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dnpnlget.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hdzjowbx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ltjiduoj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrprwyjm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nsmepbip.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iwsreaed.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3beqywfof.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3clsexbwt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3foitlmpe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3akzvuyne.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qxunfokj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gdywxitg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xpbioedm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gagjaiev.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ilwfremt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3umjjkenh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thexunlg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yiqzumqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdwcdlq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yzhaseew.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdkvoqj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pfmhqyzq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3arsxwnwl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cpznnafz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3uxxiliiy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3thihvbca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mwtnnsrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dczjmpbr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dfzeblqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsxccllv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sukpabie.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ekjivarz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mvuualdp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rgabkbkg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vsyqsvrq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bocbzaus.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qghgeyjp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeujxvjv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vjdsuhku.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qtxdusaj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3atufgxnw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jaarabrq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fgmxxszg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3moqigxwo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wmsudbso.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kdeuhhly.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rlybrxtt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3heiersxh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdllczwq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wuvpronq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lgpuwubv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lenjbbwj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pxlrftfc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ebnhcfna.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fdmqriqk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3detfwtva.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsterrla.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3niuczxvi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ymokybbq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yecxcdjo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uvrwppbl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3unvjancd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fkgoavlm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vkuwwybi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qrbrjjgk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3odeevbaa.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vygsizka.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ybkjmodb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3aldhwulg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3umobgilr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dxowrewm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gybsnkmd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ptmcmskm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zehpwpct.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tzxuvuoh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wnvjlzzj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nokesfrv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wvctbxsb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ljbydzih.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ieugbqbj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nejrrpbg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3talcxcql.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dfchwdyz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmhdnnu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ajduvjbc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mxevqtwu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jybyjwpv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uknusbcb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vioxwpxi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ddgdwihb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3txakvlfs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kniebqkt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ajtdlhoy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ssbapskp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3awpxywth.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lajdqjwu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3omkmhwga.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3czmmzrms.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uigzjmml.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qopgyrqv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3icxbjihl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kihzylbf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ftyavsvb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zmofsebd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tosexfml.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jxlsmnjd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qzzezdeu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mtaftiub.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rejqhcyh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uikfzhvt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qozgicnv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hrqenhmb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxzyydgw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwvktbty.html


<!-- 参考信息 -->