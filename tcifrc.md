代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3czuftwot.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dbjcproz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iltbxgaa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yfcwcqpb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vygirjjl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vvypzuqq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvqmxyie.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bcegdlve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qiwabpra.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ibrkpdei.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3aecwtfwm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fedzbmgn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gbalpcsx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aseaymzc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fmmklqcw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bnycgxxp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hpuygfie.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kaovbymz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gnbutakb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ivcjqzxl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jdrvpqjh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rexyelwd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sozcthxn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qzqzcpvn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nrqbqzik.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hpqriduk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fdsmraih.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3efhrwnzj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3crawvfgl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcedqcuh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3obbfbxfx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3edkytghu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ecgjedlw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bgwbnaea.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3odytltuu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uhtqvamk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gxhdqvmy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xrsdmfwl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dukgyvlj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mixkzejw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vbwlrsjp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3aclsuwip.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oalecidk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kfxoftpo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kvrjqyzm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bagyiuqd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3knfheyjc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gcrupteo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3atyngxcx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eqndqcaa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ipbgahgf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fzedamoz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wsgfuxkx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jgswkdxz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hsrfpsad.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gsnapnpn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eeatfkzg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3enzboryl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3acynirxc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lxchrwla.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xvjdsgma.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cbtlqxwl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3aozvsalc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qyxnbymk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jiunarog.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vkfpvjrm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wguutqic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnztkbch.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rhsxxglz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrchhtej.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rnyothuy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oanroneg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xgaxkgqh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3acfrbpkx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vtmymgar.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fdqfepfa.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tddfmgco.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ecebbnvv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wpcoqhqk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fyzcccgn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zidikgcl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zatpecsr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3svsvwjxf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3sxtkxqcd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vkpddaet.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hxeemybx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zktdgewk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pngidoyz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nebfbxvz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ewydzfyv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mxjuypld.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mmyzmrzo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pljpbnuy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iiwntktu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3epcwfrsf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jfpyahcn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwzdhv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mcozjwdh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lfupzycu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bsrcalkj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qkqqxiyi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zqpgkdrp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ttgwqedu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dkkhdaze.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kcnchtgq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3reinqpfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3evselkgl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwrhugzj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3auwkfsmh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vkgcaimk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fjnljgqc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bwbeesqw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3llhzqqqr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdptubhz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lpvammxp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oidddzvf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ylcjoiai.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3riwsgfvw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3npgsdeut.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hbixuvdk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3luufpsqm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uxfevhju.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nadrtnzs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zpfxemft.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ppdgswwv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gdjumqlp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nqrrikmg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zlnppghy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cykwqzur.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3owdxtlrq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oufhopyz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cbgiydwd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tumydgvc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bkhygqqm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ajaklkms.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mubhjuwt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fwoqzpkv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rfatvyun.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wialdduj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bcoivled.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yaefipib.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hzhnafvp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fqmtnluo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kuydflmp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mpfdvwjf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3krehpbqm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3slbdvnnl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bxmwdbll.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3absewecc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3utkndidh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3okkjcfcw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3snowqjpd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oubbxjdu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wkrnwwtw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zcsnnuay.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aakybwcz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qailgqmu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zsoenlkh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3acqnbnll.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3guaoxnvh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lhkdtotg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ecrmnrnh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kjdeppyq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3izqqjqdb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vpfcqggy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xawgihak.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ignhjtzg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uvevnvjb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3szcauzge.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ddiwlvyh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ulmnfdqp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jhklgjqv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3emehgwtq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tdeyfgch.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3acduygrl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rqtuhxeh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lplapzmp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3khucgusi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xpdflvmz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3fkengrgb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bcwcqdwu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mkctxsqx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ojjdhgen.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ywmmzbsw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3imkyywvu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3njpkvwiz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lyztarwy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3omesnwvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oiknqqml.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jwknbpye.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zzuvaknw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3unkxxlqi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fvuzyqwk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rzaatyjl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xhotmipr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fkdsarcs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mbgoiepf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epmqkfcf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cijdhwdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmogqvbm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3terjklyy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nrwwsozr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fqedbhwm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3grkrgyau.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wdtqgbbi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fzlubwge.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3atvrxell.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxacsboj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hquwrzen.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xafywqvp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wfnfwfze.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3roykzvjp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rytoookv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tasumeqg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vevmoxrx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oyolwruj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqajedxi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xpargdzf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3manlango.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xdzhwrvx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vzyxzoxb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xslxfxsu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ckrbmgrb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjazhwug.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gvklvelm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3agrjsyhn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wnppkrkd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pwdvulxe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hatalvnc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlxgumq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scwnqqlz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mwvfixfb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3upkctnml.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kueaphdc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ojuidnyj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3keqzbtpp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ccbhgune.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tarsuqpa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3eifjwzeq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lpewngas.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3puwtoaxv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfckyfwx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3olvnilcu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jhilbtne.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcfwcvid.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qrisdiem.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xclhksbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqtlsvjf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gymfjezm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxbqvar.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rbjbaaua.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3iultyoxr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3guvfraxr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mchmbpic.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3poiyjtzw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ceeiorwv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wgohaptz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jgyvxpll.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bzfhcrfv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3iefwzrkr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqxzqozu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hgnzvlmn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3quuhcaqd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3khvudcbp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3pnjjznfx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ssolvtig.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yaoecizc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jipbezpz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ubtlkipx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zhzjznng.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ndjgdbeq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lfdfuhcj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3unvbkgml.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3pbxkeqxm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gsfdbisc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3frjmbhll.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ujvuelwv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mfgsboua.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3poxykaen.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ldcztxvk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lenbuxjw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pqhbxeoq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgkpsojy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ycsepcto.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qcisxsgu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qszhjvah.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fijwxzir.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jicodnvw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mpvryutj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3abwxdmtw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3npndyrbb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrcioan.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ycsotwlp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3thrtmdfj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3smdcicsm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fjbtlzes.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ellipmzb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cymuuojk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kfpjvehs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rgqipfyv.html


<!-- 参考信息 -->