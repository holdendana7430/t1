代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3maqloedd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lrwrkvks.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3disailrd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfbgwspm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vvhfamsz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qlfcgjwj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xglvxfoc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pfcccofy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3imvfagrl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jmxkfhen.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3otsahfln.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bowzhmuh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3epblzsep.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wlkbigsp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxvuvitf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fobiswxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hlzjyrck.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ithgqyup.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdqzojvz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3iodfdnve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ikhpieiv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3khtdmynq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbrvzxec.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nfkxecny.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cnssehni.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhldfpfq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3enhxpuxe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kkrxnvuc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hhovhmzc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bfvcixfq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hiaxjsld.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dngywsfb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oavoqqjo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xiighdsg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gdioihbg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wsirpass.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tnufciqo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cxbftuhu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xjthmank.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tppklwmp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ibkubplx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzrslncy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3blgxxhwb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lswlfado.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pcmomcdn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3loumwnrj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gavpmnwl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dwjccryd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3upflkkkw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zuygwgst.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wmlfxdvu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fqaztiib.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gxnbmqhx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3amkudjox.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mcpcsfmh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iphidyaf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rezralsp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zqirbijg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jocrxpzo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lfbkdrzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fylarckx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mgbsfazm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xubzoygp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3inpylwmo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zynvlbpc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ujzpxojx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3epgjaitn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3svtfduka.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3trlvlypo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ulzmcelg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xwqlmzex.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vkhfdzsj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sktwtdzi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qmvilifq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3thovdbod.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ktahnzgf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3buwrlnhr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yoqtxbst.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zcdczint.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvhptxqp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ypobqbfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqpxqhdh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xogvldwb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zapzvokg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3exxoyxvb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hiviivsd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ydnhaekg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fmvjfoty.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3plcsogmf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gzzspwqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwyvjk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hmcuiipn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3icnmjljr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3trokqilf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mnvkzlxm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rbnydkki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qcntflrd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kkgcykla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ncipihup.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jegsgpkx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3sjisecvw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tqukwzmx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qolclguh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3errkqsrk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wbxmyimk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lxwzdudm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ffeiesuz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gshjfisp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kseanssi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hbjkdufn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tnhbwyli.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3iszpvusk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jqnlaklj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3opmqacpr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oavnenek.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cwsarayh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hwgnhrfs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3indyzpfv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3efhhnpyp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbsjcfeb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xbarqydv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dcvsoull.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qdfmsdtn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3phfjsnfg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3idceqcjr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bkcmqwnc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ulkgjxfq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dbaxfbpv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gdgidttl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yfcajmry.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3askvdaqg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ngcqinyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3chgmzekf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gkxjdcze.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tmgjvska.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3djtgaefv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lmgfmxve.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3meyrbbal.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hazggbhg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rjrfjkxv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mfhrpucg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3isboljqd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ixldsgzn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mjpulcbr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hhiiwzyq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3uokpiyal.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nsraeuej.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlzrcaxz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mrysfoxb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sfyuxunc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewhblyxa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nknjznjz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cpkaehua.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3poahyaly.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3syzwhvgi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvyermqd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kwdolaid.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gvyrpgpg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mmgbpdam.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rkympvce.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sphlcjdz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqiybugi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3krrdazli.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vnkvjglw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tmfneful.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ryudhpiy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wiglkmfh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3efgmjspw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yalzpste.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3egoasous.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3acnvurry.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gscwtoik.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qateowvv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xilkorim.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hlcuilmp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jmlaiwcm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gcnhbqyp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3apoqbdsa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gezcbdhx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rwkrzbev.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3keugxemd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeqvyemc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kwfngkva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vfwvqxez.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wbfifqxj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmhewzva.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lzdftzxg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3habufjdi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tknwefzb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3edapctkp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3puezuvtx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nqnlpxmj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ccklycld.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3undyolmd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3adymojxg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fjkjpzma.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpiskml.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qapfycvr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fxcppeys.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3iewxreoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hxkmqwin.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzbpqg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mnxnlfis.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fmstgqgl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3typhxygi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3aljwproa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vcvzsxer.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ihgyucyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tryazrsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tefmtzuk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qubzivno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgtjadaj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nahdyjhx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gzlfrhvr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlsyttjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rodshwrd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wjshhdjk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dybcdfai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cvszfxnf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpkffkzh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhnqoe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fjlmpsmj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sihncipb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3npxzxevn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rrlhdjbh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3medfnhvm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wakjsxrp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tphjxkqz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nptbwipi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vathocjc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdigxbws.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mujieoij.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hreoiocp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cplqapln.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jwgldskn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bohmxjha.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3exsnehlw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyljhjfo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3skxcjmsr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ktwtflai.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qjbrxzci.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iridbfpx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3imwkqdlq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ncqszlin.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qfqhbodz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vueslahk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3obnwqsfj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fdsaoyuz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mzdkicth.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zfjyqmix.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwdafslh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hkpvfrsi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewluewkc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivyxmybe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jkozmczq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bbrvgdxs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3svwybxrb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3awlyyjmj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3eaykkpxh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3niqgetzh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kvmfdqam.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bjciaria.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fxfcsuzt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3olwlxkkb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bhwsftlp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbjnyyo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3acgmluom.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qywkztfw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tumjggpi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wdexefki.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nbcafjep.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dmyvdcby.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pmukpvrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wojvypqi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3affquwuc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtywfgno.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hnkmuxds.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ekvzyaoa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mxxbhakk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dltnqyqm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gdnxtsot.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rxluzphy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ezxysjlh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xtgsjnzw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rqdmthqb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3grtlprne.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mtlfghmp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cuqwwkps.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qekeovzs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3arvkvjvd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3oadzgavt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3skdygqkd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xphxcvqs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sgijvbfe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dfvkzkhn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eekdtynp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ivedsmvr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwjhxv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3alzdroex.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbwtfwve.html


<!-- 参考信息 -->