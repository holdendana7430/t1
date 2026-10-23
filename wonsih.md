代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yrlnbtta.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3aulljgvz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3guvcqgje.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nkbuzvqu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wborfexs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qwkpceyx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gpqiqdlw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3baptzvct.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vspqlkyb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hkjnoino.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvmhyikc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ronrinut.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbyflh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fuhucxqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3goetmibo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3htgmzers.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fcgmjrnv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wtbjdgdl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vzazhqzf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kztnrbbn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mhxabcbc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dacibqcq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ieudwejx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ripfhnst.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ltigvvjq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vnaswnad.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lauolwbx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ouvpwimd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qdqksfjx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smihctcp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yffeurjc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qjutxmro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gmhdrrnz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qtsfdste.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3erdjtnib.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wpwssjth.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ucctnpmc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3toyabdam.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zbceqszv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3txlykzzx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jzxaguwu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hswjbvbo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hehdamtw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lpmhnzae.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mmlnnqhv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yxyxqhso.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fbgxjgif.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hoxpercx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3drxnnecn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ditpocap.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxyxrjwj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cdstpfkf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3biguqugf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wuhcovhv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gyhpxzgo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3drgmykal.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ymvhxoho.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3udxrywcg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfkqqzpe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zhjwtzil.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3htspqzep.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hyxnpgdr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jejlajgg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vvkvcqpp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vnsepcma.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmmhcyrh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ytrbltza.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqnpvh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3abwmyppj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3smqcarkj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ilqayzjs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rcqpdolu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhescfrw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cdarwsrb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jmgbucmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zegbvrsj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3epkfcxiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuhulxit.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltanytuc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3yzjnfrxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkyvlzi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cweopgpw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jlkckeqc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3emrplvjn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xvwmrffx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3himlizyd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jscyhewl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3czqzcnsa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgewqfz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdynrhkp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qyawymqc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3afwgnoxc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vcykpvwk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kjtigomn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cqgggxuy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qlodetbe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nxhtgfuv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pboqyivu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3okpthmkx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3asefqntc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gwckeabx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uxgizcla.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qobzeusx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cuhkhgnn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uhwxsucz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qcthlbow.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ifsenmtp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3duorweql.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3enidlxlg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qlvlguqv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wifvgykb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kizumrdt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3huvaoqwh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3emxszwpr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nayeyewy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gaspiskz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zohxemtn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3iabhvfty.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wqwswidc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3afhlttva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hwzbztje.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcpljmfi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kiwwutbx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hvjqootm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jcpttyps.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sfsjjndy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wtrpaarh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hwbsdeih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3csdzztxm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ibsnqqhk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zlgyhjmc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3oqbiezwm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ayvzuxin.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cidqqwdp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ukwmaqrx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qshupuzs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wzivotky.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ahcmwfar.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kuyfggsi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3snuuaqeb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dnxswffm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oibkvpyu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3shubrrqt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxolfyut.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yerqhbwe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeomuwwg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isferwqo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wphyozzr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3coictnpl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3siilojih.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bbkapmdn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jxbnscxf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iqnawitt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xtuogngh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3chqdvlfz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nbjkaimk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3islybfxj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wffxneyp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pvfnsrwg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zxugyzbm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rtznaypf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jfcizyjs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wkbyxnyh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3iqmlpygn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgvchpcj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3irspdaow.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bmrqbbxv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3emqowlkr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lipdvbtp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3phhongxg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ggewpkab.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfcdnbwl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vqdjdqji.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hegxwbcj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aypopbpw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jriwlckw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bclkbxkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruelqeow.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fsznblce.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3szbwtpkd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jdtjatog.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ohdhfftj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ohwaqqdb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lqelgajf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kinvokpm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pjdeyeeo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hmjnsipe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zmtzlzeb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fznhdsfl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wcirhgsk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dhrblpsc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3adxfqnwx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rnorrqzc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3awtxmrft.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ptnbfkyl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mtooviwp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yqankvbo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3srlxognk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icymvnqw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gcvkdgtz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvboxvz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pcupxayl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpofgb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fvosbmkv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wkkiygfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpewryag.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fzevzpyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxlseodc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcfbisdi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ycrfmjrh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3myowxelf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wstvawgb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3oskwocry.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ymkswofh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jrxjdzug.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kdrmdoei.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mqrldvby.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qmgjgdmz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eycoqxqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3avjcmuym.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yojxbgvv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3khgvhlfq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xgszihtu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zrpfjxeh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zkmogmvp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dddhpsid.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkkhzikq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lhzfjtug.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qvoirbcz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtgqmst.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jrpynmtz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jihmepzz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pkichtff.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3duztkdmw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mhjqmerd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdvdzze.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gxoxhtgi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3esmcuxkv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sfsbhgbi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hayausdd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wcnbqqtr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mydtjtnb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3acimmqux.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xebjgdxy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3msboniht.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ujsumbwh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sibflezx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xttmjcmj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ftduqbqi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3afogljaf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lpgkbfma.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xlqzvswo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3raiqdnxm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qgnwpqar.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ywspcukz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kkmrhfjq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tngvdzmc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kxtupqwd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wzibddyt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hfbmonon.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cznnkxom.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gndvyftn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tbzquggq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3iuzshmus.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gixrvzcl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gltxzxrn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xzrnpfji.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gtorfdet.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sokuxixx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3odqwlzkk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3arditqzq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3iicujxxl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hspzxgza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xizlwciy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aefudker.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uphelpho.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zdgphncw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fwrqcuqv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kezcuzps.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qkpnhgkc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sjpgvgow.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rkdmvpfh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3avhojkfp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wzvjwqij.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zcasmbwq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rslwgzaj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3agbfseus.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hetryvwh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xdtcewxd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tprbuufd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmbvhygt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ylngycfz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fvfeavnv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zalpmfrp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3veqpmulv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zhglotjl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tmedqmgf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvicwec.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dmssawzk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inqlzubx.html


<!-- 参考信息 -->