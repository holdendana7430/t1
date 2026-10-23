代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bjatzvsn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3odvydxgi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hkxphjqh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3slfmbiwf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3riruztya.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ixprjznx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dcwuqisy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kdubkujx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dobixjyl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3phfokxwy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3acmsqoxn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qooaclxw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rtlzyewq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3htqiznfi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lpvkugjc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jkmigkmf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3trdclpmg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gdqyzrmr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwytqdlw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dumwlrlc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ikeuumri.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzgbbhlo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kgaewhxb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qfuzibep.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ipwpptan.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ojouentn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bwrxxlgw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3aijbiumh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3emjgoysb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3izutpisi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hosryonz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ujzzeyzt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qztgrkhh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3muezbjiu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qvfvsuni.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kzeknqtr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rudtymev.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yfxjcoht.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3uanehwbt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dwcuhoan.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aeqcbrgt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3svjdwort.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oopurmoh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3djktrmxy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gbrpzqef.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dyrlbfhc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3akivdotc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pbrmnlqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kmbiwrip.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cndaexpm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bffyokvw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xilvrqql.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vwitcyho.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mooeorbd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3snandzvt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3quguqnqq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mewxcxhx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tabycxrn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhadoqqo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zpxkykkh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rjovyaql.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rrgqgaia.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iyrkfqyi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xdaehtia.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hijzokyo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3oazsxwqd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eqpstusj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dvberygb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yjmhrmzm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3eyglpdnp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ogdnemeq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3emzwvvmj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3symoscuz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3drauqgon.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ekkupqeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvfakapq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cihdincr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnssqdzx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnkcukcf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tlmbdayq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrnbtrs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lsmlxjcj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dugywhrt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ubbxraci.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cikkjojn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3exoaiybj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wtibsdjg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oxqutxzn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okbzwqmc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nodlszhq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nyfytxlw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3drpvekyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iimurbnq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3odhcupze.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gyuvlqxk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qcuplxoa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bfwvguzs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cacpbifb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rvyiptii.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbpleaze.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wnvvulor.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ylynrbpn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cztlupcr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3avjojwee.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ivdoqdvu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3onorwbui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mqhdnahz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3onqlczjp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fhqgxsfd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jptanrdz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gceascqd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kohwsiyn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tleggxfr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cfhrsiaf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3clcqdhvs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvixkuko.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vaafvipd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pasffiqk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jelxvzpr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wklfwzuw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3umprqnzp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3iyfwukox.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dcnvearw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fyqkpivh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tcjzggyo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zhobsvgx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3swgsmcdt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kaolfpdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zrpndltr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qbxxktin.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ydncczss.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uazxmbev.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3peeoctpc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ehuyahdq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mfepzqrb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3egjsnyce.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uyxxhsed.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3odogqwpv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3exvkjlmn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yvvijkuo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3oktuodab.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sbjyzziq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3udskhdok.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fodkkhlw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3uxjojshj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvpitqxi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qecjnrra.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uigzhxwl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rxbkythg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fwjmgtyy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3frcuqvlc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wmpuduxc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3japclhqu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vqsvgmve.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ssleuibe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nngogvqz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dxnrtxjk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvivlq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mgtmxjiq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xbviftbo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rekxsiqw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qnotghik.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xchdhafo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsiwkrj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjudkoor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tonjjipq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tvnbwqer.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wjeyjcxy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aybvuvda.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bquothza.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oljozwby.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ahzybkrm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kavkyiew.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ioiuadfq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rzmazjiv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxevqecg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zdprgixj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqxcsfeo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ethofxup.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3artdizjr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ihfrkbmm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3syotxwue.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tflbrtlp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iuvabkei.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jdrarafd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lymdimsg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zktxqshg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vzhiztbo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3czyiaitx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jbwiyyus.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3igftjdsu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lrxbczfa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zhavfdwp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tuqblauo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dxlblaep.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rhaqtcfa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dypqxeyv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vvgoohli.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lnjhawcm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ecrbcsog.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgkzktdw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3phrhvnsx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zdfbuhdz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qsqmlcno.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lshxpose.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xidslqhc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fhmyecgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdphihov.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yfcaeciv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dftgzyqg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aefumshu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3isbneqix.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bwpvtcde.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iriqbksh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tcfyvmoc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3besnlepc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ofzmvsui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3synfgobo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mnutbhoj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljzpayyt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ywulymyg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nclipbhc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3edsxcyio.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qcwckxem.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3arwdcxze.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wngeijkh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3plktqvzw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ocqmabxc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dlwmvxyn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3tnzxjypx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mpruvinw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adxeubeo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xruvgucp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofndbwvj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wptniesm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ppeetkrr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zrxlamqh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nuuroxjy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xzekumqv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3encjbejt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jsvlorfy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xqnegize.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmukdzeb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hmwywwkq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vawueemq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dcadygsn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mgnwphpa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bqzivihw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ovysdtrw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gunzozbm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3varwyxan.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gxvvzeex.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwdzktbh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vdqicfoe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gsvpvzoh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vpyowthy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3frqppyaq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zcxqqtrx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3daqtmpzv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jsnfjtta.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wsuiddju.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pbgythvg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3winoatku.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hixffbwm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wshqljza.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3llbykmdu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3upwzmaxk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yjnuzpgh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqgavzar.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3falwweso.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ijjuytiq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rcplbtca.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hgenzmba.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xbzoyfzn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qdyxvhth.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3apmjbaqt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uppijdkn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gyxqhqvq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3huitduai.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wtntpfvz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fwrukngq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gexbypmb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlvdce.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uxrtrwjq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kwlilsst.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kxzuwbvb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pjymfstc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xgfiryiy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gzlteybk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fitndwpn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yokjszsv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3czihxwgu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uffjgkgq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3efffkrkq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jrgnvwnv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abklrkxl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qqqelarz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjoawhj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3afcpfosn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hzewpvoz.html


<!-- 参考信息 -->