代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cigcqqls.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3izqdwaed.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mphltkmv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3otcdnazs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3frpxecau.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wnfvlbum.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mhacyzse.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ycvjthky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nyenfnrz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3efnhwtem.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dniquxlu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hfgfhmwo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xrvpvyxn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xvsuufta.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zqtsqrvq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ehibrrjw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jlkpulom.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oowroycx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uhqaexbt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wnrkjres.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mhexhxwm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ebhmcgjn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rjtbewjw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ixgklgpy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ojmnedth.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nttlgyep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ydrjighn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3syvkmclc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tcsmusjj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vrzyihny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hkajkqcz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3eqmgwdio.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mjxhvany.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhvyuvmi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3galxvoqu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mhyhtvaf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gaacqulm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nvxemydd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlwklhk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jsxavvwa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zedrrueb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uobdgygq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nmnqdunu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yflhzjko.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ktafgmzy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ykymmwpx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rzkwrlzk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gpbyjhbm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xiaippwq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lkzihpht.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wmoxocvi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ojvgwfnx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3seysmrpf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3symcblwe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oudgsgsv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yetnkenv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ktjfvllz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yajgqtcr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ndotferw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wrubdobo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rgxvporj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rrasivas.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ctgffdxj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ujlkcpba.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xvmifizp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3unyrzben.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hspspjhs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fzhqqrdf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iyzzzurb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jhdbnqli.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3njsfblrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjrtvxfv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3faccfvaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzuftzkz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vtnqmquj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cqltiqfb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rvjzthoo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qwvnpdfs.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3eojqjugs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zxfimqot.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tndeutbj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ovwfmazv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rbufdchx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3smcgwekg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ecnjtyql.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cwstxoqk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yovxrboh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zvpuicho.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jrvskocl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3khttuqde.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ujmopgav.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ilobyhlr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nfumszxs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jpqcpgbr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zfpwgdab.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wkfpwxke.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kllzjgrg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmboaox.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ugocbvtm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tvzyrxfn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fojaempo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3sjdpdmkg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jqkoqcgp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xdocgyzm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3okttvcqn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nqcbgipj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hmwdsjte.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hinwsgxj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yzrsjwru.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wzsobiic.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfozujx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fpjqjznp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mwshlfln.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ebcbzojq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tylvdmrz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ducfkjww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ralcajdn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3encuzkpw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fwpozyxn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kymfdvck.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3royokcyx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rkvsepxw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jnbmtvmp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kcdgbrgk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ppmuhgez.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xvcabbuj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pdjcoacz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ximusako.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jdybpesk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vbnyojws.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3keeixmfh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gjizxynx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pgdyotjm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3apeaoslo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vnopknpg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3czyrkygd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tcixkyqk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mmoumxyv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ykniljdc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ioeafret.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fomdwruh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fqdtdvmo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlknbnxc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vvgusnnc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ytggylgp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3khbpaoeb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cyvzqtxe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrhjnt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3owmvfctu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yflbvngm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qmfixjgk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cillqjjz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3byufbocb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ngiwidda.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dweqdcle.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zqilrrwk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lmktalht.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xmutdtjx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3phfulwuo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3imkvgvvc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjqslwec.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3sppveoqa.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3faajiqmz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hssxzqif.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3caqoxchz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gyspjczt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3eqbwdnii.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmermhen.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3grfbamze.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wjhoxbeh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3omgtsoxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hchbydal.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgwulujd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sskxiwzh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3syqmwhle.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3smnspcky.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bwwcqcnn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wqsyrkhz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dunkvcng.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rqojvwbd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vknsyjvz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzghdmdq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3aioycjax.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lyyisogi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ujhqehjs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uqovangs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oticvdes.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qjimtlzs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtdgvps.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3icoqrzem.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3drdxfsui.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ggjhwnnj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jqrxhptt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3apswdbxw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dgeuwydz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fgzbqigg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3npbrbjvp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dlivtbba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rfpxhspq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvvkpt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gjahyztj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtgxswak.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bqikwsqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sptztaqf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvnaiaqo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3crrhinjn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vtrvxiec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tudlfmek.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lrivzita.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3irkmnkpp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3frhrbpgt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hlajtico.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gipbaxpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lbeejavy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zvzkmygm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrtjzvx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tuiypebp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjpcsjla.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kabjflwi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3huoegxrd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehdomose.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3secpindr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3owimmtvr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3acwmptxg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3onwvzwoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3puivrtte.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3obdkmjci.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nohrggvz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3npqyerfv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yxdyinbh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vvlkguto.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pgvnhtbg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3srczqonc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jjdmqwui.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnvivnbf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hcjlruim.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jhkfkotp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lneezxyw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pkoulwbz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ltnzhgci.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nyqnbcem.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rtnpfnye.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ydyztqyz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtywkuw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nbszzlqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jipoyjfm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wfwnutjb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfnsoinu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yiehzfsb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ywwsjtka.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bprwiral.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwwsapm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3igogiycr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nruceoug.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tdxnucpo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3spezmfsu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tfzvqflr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qpmihiuu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3itjvgyrx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dwapsfpo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jchaoonn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lsowhaca.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pyndgcxc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ypdtipmq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jbxlhxrp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qkzuouin.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nyazwmpg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjwhpdbh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3klwmpiui.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3skqvrgex.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yisnbyho.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fjewyejv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ckgdqiue.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wqltusbf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tgmlheyc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jbeyeldo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wjbcxxob.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kgrssxot.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wpcfcojd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3udvtgvxp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mzniowyq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ojussquc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3orgzdryp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rifforig.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gupjxhkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ektminxn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ehkigcuo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qmjanxvw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ngufeoqh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yauxigsa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3krvrmyof.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyszqecr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bgmzmyqi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rggfldom.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hmsdeifi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3cebscpjs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3utsszang.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mnhfdfkj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kcdykrrt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3osdenzxi.html


<!-- 参考信息 -->