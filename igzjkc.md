代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tgiwblxd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3llutlyyq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3akghvrlq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3phznaxiv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dbbtesju.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rfeqnpmw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nvdfnnvq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rvcyficy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3difopvyt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bjvtmteq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3diwbrfho.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zjkazmwa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bjtcixdm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eweijwan.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oflddtjl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wnzmzqii.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zlxitgtw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3euvtuhnc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgsqmlqw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3drasjvog.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ixuyknnc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioypfejf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3twbhnsjx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ohnxlqdn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3haervuua.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fukahlfm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jejeqytv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qbyltokt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cwfptebr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vgvpquwd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zmclykqw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zunaevck.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rijkzwqy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3prumndcs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hbuogwnd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3moypraco.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3koawxuyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxyczyga.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hqvaapee.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rudxhllt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3smrextwn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qkkibbns.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3oxiyzhsp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rkthrmpf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vfbtoaji.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qogccwzi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bnvozyib.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kvzpfknk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bxmqbvig.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rldvmyym.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkrjxiry.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iusjndfq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3csyxranc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3plpxxyjq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xcyjdixy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mtyndcfz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xjfjmakn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tputmugm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3docnbqdy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3houapuhv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wmesrfft.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3etnugxod.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ezhjzlgf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbvwmhcj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3haxgcsij.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dafzxldd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oxtttmil.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qwhmtikf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gdxihwuc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gxomgfek.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3oyqphjsd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3apruimwh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3agtvptca.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vmbefqpd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vycagrnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekuxbjrs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gcotletl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3popkgikw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pgakediy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uixwheka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3weqggcpf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ciagtavd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3aymsnnep.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3tozmhyyd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jitbqpur.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bjopudca.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hlwviurz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yludjxir.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgzggpn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bzhixnhb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bdstfpft.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cdsbmffr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gflcatvd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mulsiuth.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jvdblckm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3msmucjnh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tyhsezww.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tdxqesem.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3twvjjwjx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlaskkvz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3sxeomgzh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cnesflau.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kesrtltm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zctykdkn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kbdmfmsi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qnziwkwe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xilpvrti.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pbmpcfdf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bkgkuthh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzvnhiaf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3trpltdsl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cnxanuwk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljegegkj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vnpyxfij.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tmnpeemz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wefoczzf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qawueobq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gbkhzkrb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fvbgtxqk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vbharhwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zcsylsqt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ukpofuvu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3culnmbwq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ugmatzhw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3twwfnvlt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lemscxlv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fgjysisd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qrtcybqs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3khdrgkhr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3usoqxowp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lngcxwhu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zehtgbpe.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jrfukvbx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nisnzphn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uikljnio.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3haiqzeuw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ycozushz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcpvamkn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oumqjzko.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3isqjqdgl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aflgxbhl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3toevhrrk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3trnzkrus.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlwwjrbb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jsgiesya.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jbgfnjgh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3krcctdqc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3erhaywjj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jlodpmxb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvllaoq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dcrjizcp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fygmqgai.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uhdgqlar.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxorsuzp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3guonefsm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zeoljizh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mlilsotg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fubonvdn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3avouguth.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lxldxisw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iknakiva.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zcqgajfi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3agfzvqai.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rdozakil.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sqxzpwyr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3srbycypx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3krgedqfd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vnkscwcq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aezvfxsd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wrhoalkd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bjlpoawl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhiciabu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tybmrfec.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fzwyevsf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lcqubrpv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jdblsauj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kegpterf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kffalkbe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfqejvus.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rvioksmy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lsgpngsn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xdotacjg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sjkqxism.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3heupxiua.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hurydgaf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wrevpwld.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wdevguud.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xivaggsp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gkkwtvsq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3htbmikqm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3njbplrlj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tphxqsfu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cszzredj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lakmargu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krzylivj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zdsmdlqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3bqgvigpo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gsmanxuh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ebdpnvcf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kiaeysxu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3enduhanj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tndwohry.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vxgozezk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxevftrw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vltoxypc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smzfggyt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dacedhtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwwbcxlo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpqkhtvg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hakwsrjl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oetgvpss.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fqggmtbg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ccrvpmnm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zxgfbikr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vfbcnrpz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lffvaach.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tgezebei.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nmrnxkeh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zkncpsdt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iviljioi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3njgznull.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bsghfpov.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bohnshqe.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ikeefvhi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ivqwggzv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hnkpjvjr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ktpkrukd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ozuepsrm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3notqtsrx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3asfqfmjv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ugtvokko.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zeiczqub.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kezwtszd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkaozucd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fulqtzka.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vxerliqt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bkmggnax.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jumdvrfz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hbgtueir.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hxxtuhoi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vmczdzyo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wuazxpkq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xkqeiimn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vgeyfgoi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3syyvrbxt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmgatgnt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ghpnbgbp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wxwqbuzs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pnhuajmp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbwynu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3idcygbzd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3unodyzlv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bdgwdxro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hujxzxvj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pgykaeio.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yocuumda.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tmqoeyor.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nzduvavc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bdaukbnb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjzbxvw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kkzhkgzm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltniqien.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vkkgviuo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mctiamah.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dazpznov.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhvluze.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nxznnvtl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uufnuvop.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3izbyaojx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pitsodiz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hkfsyonw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3flzktgso.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gyiadflc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ecuhbyzv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hupsmamj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bztgtnbv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vtiqxnmx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nzzqvxgm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pohhjbqn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xkcgerdj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ymrseytj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3yxpsgzsp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vtjxbfok.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ehzdlmsp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sefqecpc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sshnmjeg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kaloocpm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cwwvkezv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3szytsjjt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3teduspgz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpwqofvb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tuussiyv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3daijzajg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xaezbiks.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lsnghioc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfagmota.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qabzscoa.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3syermkkh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ehqfhrix.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jibstyll.html


<!-- 参考信息 -->