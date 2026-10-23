代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xkmwyiwg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zhxiaesc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uppayidu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kbavqylf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shvdogtn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ohacplbx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3shgytjca.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qxftogdk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dcazbypf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nhsgfdty.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mgysdsmq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rcstybex.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wrgsfiqt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fzcdgkwm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3npeapxie.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3imivhdqi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ecwedsot.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmrqfxpb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3teuvasou.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3plwqtdof.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jjqtmviz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ybieffor.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gsppkddg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xhmixqbh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3eqyhazso.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ivgrhcyb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fcgysdhz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xkdzjfdk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3shciamyp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sapcqeob.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3afqaujes.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ylmhplaz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tuvhisel.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jvfxlnvo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bgyrecay.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3krsayjbc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3iagnjqsr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3unuskxrz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3khpobomy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hpaztzfd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3putwpfwl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dfxkqyvt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mrmdbeyn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ynuutiug.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kpiyjdrg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dznmugkr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pywkxcxu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iwwzrzlp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kxlcglzg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rtgytolk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yysunbxt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hiikrjbo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tlnguwnh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uylzmevi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3evaqwhwq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3airaiwfx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gpwgwobj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bpdffzqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vqapknhj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3egpwlsua.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wivsmuuw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mxrsiafl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nloglftt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wxpfsjcq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jzwczyoi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rtidleal.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3oidkvjpa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jjrrdhbt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bymitpyh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zzvjwbea.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xcfprzdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rofidumw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qawamjhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjccijph.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bawsahkq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3titzmhnd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqdexxk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfaphp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3czgtefrk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fxzbziqy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bhpukjpu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nmwctclg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3krlqkiif.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ybidxqli.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3shauarbo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mwqdqgks.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3divxiwls.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yrsttsbo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cnefybyt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jpjveixu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xxveiyzy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kbfplitn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uohmdzsi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pqymlpaz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lupebufg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqkxkfzo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dailxvhm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nagaiepg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3laiwqncr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hglzjlmv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hakcqftz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpqymblv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uzaovbrl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jduaeybr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zxnfvomk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gqagymku.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fuskrqky.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3duwvkjew.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jbusznvn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3capbekwi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3krigqusp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qegvurlx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mpnjrgse.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3siogiltp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rmkukhzo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wmcmttfc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zsuhhzdd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ajyasesh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kwlrrktu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ozjuzjzh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3swzennmk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fpokfcrx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ntjnxwje.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qriuebqv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xiyydgkp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qwivmdvm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tvsnuevd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kgvkisof.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3avywbukk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pvumjput.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3foansqmm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ddjwznbx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bkgzfgni.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvrsnkou.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fhvamxwi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dnstsfgg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3snaakoqx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hhquucau.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ddwchxyb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xoxxvabp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3iymamohq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fbqjrkrk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhqdjzcu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3sbgxtjmx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eprcthqt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tgascldi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yjqzqijw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3okbrcfkh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wxfgodpl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvsqypbd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rfhfvdkq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vktthben.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ishfrslq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ayqcywbd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3swkwchnb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jcnoixcl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nkdhgnzh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sgxegbhb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gnxvypnh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3scqvgjdl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmljiygx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhyjwf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3adwdjlqx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3smoigkwv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bryrpygd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zjuhqnng.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xcxpgqib.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uivlopgm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dxmtgapx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3karwwbxk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3houdwowl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3abrybqlt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lonazgbc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3knhbvnte.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oevrqauc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wcsetyma.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pyoggzlt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtcsgehg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3coyjfcwn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3llflhbvu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3flchvbkx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jkuaaazk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hfgwfwpg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3svmsesrh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3sutxbydo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ckhaqmtj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zlvortyj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jjerzqnv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lkqliosz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bmigldly.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3perlubtf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ddiijsry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgnwjkyx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bunhtwen.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ewizdmlp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rezwbuuf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ccfncqdv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xqcwysho.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rxwjkeei.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3loehgcdo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gtjnbshk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atsmbkmv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pboxrawy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzlemtwu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gbaolslg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3siwghzte.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qasrrubt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vepxrecr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mmfgtpio.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wdgemnqa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uleitbud.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lpafjhri.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yfqcyevg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wfxvxbga.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sblzszqh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmfxrak.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3enmbnvdh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3geagjtsk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3usumdkso.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vvidanlr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbkjshje.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kfypxcqo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qmmzztip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3njnmybhs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xondgnll.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vlnyticj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kslpxplo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujtffzok.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mdlnafgc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvcevxxl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pfyvpbne.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fqshvsop.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kpusyozb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ochoxdep.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bukzrtum.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zgzxkwcf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nvuipxax.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yjuqonnl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xmvwccgm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eatlibat.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zngfpbif.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqzronlx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bebiydhp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3flyvtgdq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yxlpncmw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpuuujte.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dtmwxfyn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrmictes.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jivgxwoq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ulczdktv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3syqdbsfs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3usfrymnq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jqepckxj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uhcmnbqx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xmftfdns.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hbqipmqa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ppuqwsop.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qalmjpcj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3toudnpdv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jwbtlqga.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qioyeptx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fctyvncz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fsecuxut.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ljqhcgsd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kdixqzxg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wednssvr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3szleunrs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqckdaeo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zywjobpa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zfhflmrb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3osriuhfs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uwbcjvny.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3blmvnlxs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3guafgrwk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uywqisuo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3diuogddu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yombcaaw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vjuewjdy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wkofakdb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3oblobywj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzgfgd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wudzsqmr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tdurwpfv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3sqbtgvrl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ewwhuznt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3iqvyhkac.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpwgsnim.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mhjqlcdp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovbhswom.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3drrraaro.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xshmjhwv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbskvmp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgrjxtny.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdqznjrb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3czxbwavx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivdhblev.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tbncmnfr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iamvnqzx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3azwyanpe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cihkghjy.html


<!-- 参考信息 -->