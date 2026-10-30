代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gsiuiwgpr.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgccmbr.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gcdloactk.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfumglhg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzpvsiqc.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gikfhvmti.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggebjuyqu.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbbophxbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcrejgir.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvilxjrna.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/glhxiludu.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbahxsil.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gwmyjmput.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqsfjstzz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkdehxr.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gtjdmrceo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdzveivz.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebkcydvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtvxmwaq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gumtxqngu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcpagetu.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfhaaheqy.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gamfirxbm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/grcvwtmap.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvievusj.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ggyenlqvr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gclvwywqz.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqjoilwg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gfnebmxne.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzxgaihti.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvuncmlxu.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopzsaeyt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimvrgiqt.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gcqcubvfb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbnqqcazm.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrgnpmu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpqlobhx.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gswwcxbrg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grpfrvkne.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktgksej.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdltwieq.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdmrxjaew.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaakjszg.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ggodwvgqf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gowwspmgh.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqhdtgfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gajdyjcjd.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gotywtkwm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkukqpao.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gujohvcvw.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/ggbeqiidz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqxduzge.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqltmsdp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glchtaakm.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeayzycc.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gkxloujvt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqnnvlxn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvbyjbsss.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtxjdfvt.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjbadfef.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfionqe.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gclvnktfq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmtgdsmgm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpznqyqii.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfogguhfx.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitspizu.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gqtofkxvz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gruqvkztm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gpocyhwba.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/ghvaxlzlv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmxpyyuq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/ghsxvzwxn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gfnhrmatx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gegmqvdpe.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbecuugow.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaykyavum.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glozsnjiu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gggvcmegh.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvarkagem.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goioqccpt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrkuymgf.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/geumfkhcs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkyefaf.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbvzklez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagzoedwf.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gamxdqvwb.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggqnabcgv.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gsocnvsje.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzirxbvjt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkkwfdqx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunklnqa.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gggdzurkz.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gtllosugs.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxncfwdq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbtjtylv.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkerdxkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gvtllfblb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/geukaukjp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlobedmp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gaorrlaec.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gehtrrvth.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyplwoghs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayafmsnt.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gchwuuizp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gnncqaalz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gtheewxgs.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxzgbplz.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gegpoqcuw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqphpmyml.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gphijskca.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gllmlfqxh.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggcfolzok.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gliqqqydd.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfczpqbq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gmagcfqvl.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gkrukgesh.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdbsfeuxg.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gesugxvza.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genkckigm.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlumwmko.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gnltutxzm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimvhsdad.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlneueqh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gkwojkube.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrohloao.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdffpouao.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gjelldqxd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprmbzqz.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxpupiyj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdbmmvlvl.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gvnciyozj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdmbwtm.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gaykidych.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glnhlonzq.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxcmjpml.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnabcvac.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwjhrhwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gjpjaawjg.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glkddjdgz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidqdysl.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwozaaag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwfkkwhap.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfrkumgix.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gzqmlzixl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfueenp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzypmggmj.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/grpuqwiwt.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbeqtojhw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuidcfgv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrwxoswh.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwuxkiej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqdnfhma.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqkaalzcn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gargwodaj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcozivzxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmvggvhe.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklddzcxc.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvtdgho.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gdmbxqnyu.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvmoolzdp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gockfqsfb.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/glejanbds.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdmnyizxs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhmqntfw.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbtyyfazv.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/glbwnubbc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gouknaybk.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpopewlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/goxqbucym.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gafpsiwtl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmweslwp.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/glyfurvnf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsudpkedv.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gghgehevr.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjnycygt.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gbaaagtkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/grlrlzwaf.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/geqlyzhqv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxwixqtr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gycuvphce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdfkmopj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gswfrevhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefcgzsk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpqkiowh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gduohcoif.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqkyydfbb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjejtnvoa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxpswurc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnllpojo.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxzjokvs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstumsocf.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gjxtzrotg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvgmyog.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxdrmrz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gpmskxqqr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzzfwjttd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gwxakgtvl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gypsgkbhy.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gtnufurbh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfvbxlf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtbogudiw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gqksryrqx.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmteduwx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gosuvkirj.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbloxnvfb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkexhyzj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfqzuzpf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grscgnpoy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gjwyivjxh.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxhrnwu.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grpbxludb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/grnmzjlsy.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrytskh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxniwuyoo.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsbebxyx.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gonuebweg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/goipabdev.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjilmifpd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/grshoecyj.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzuwxdke.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gofwktpbo.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gepfhcusj.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgljgpx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gknjnrbub.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grefeosay.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcwkdsjck.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqpmbynp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzujyylac.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grpoinpwv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpegrrsia.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxautjgis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhbswcxg.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmmosaro.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgjygipb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkmsmaxm.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvaplaxi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfcqaiqy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfirzmhuf.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdomukhr.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcgdqxfg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/grdcrstzb.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gifqdowkq.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ggjkntkxh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gohfqfxtw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjvtuoct.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldgluxnq.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gegmdyeic.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gwxijuiuz.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/godvhhlze.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaflgkvny.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/grkazqdye.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guljhzfxf.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gmfrtytko.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyoqkzlpy.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjfjgephz.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxbfhxu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gglnpuvqz.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswonork.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/guzcezvmk.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/glhiqfocy.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuzvyorp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/guakeagpb.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/glplcbfkj.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/ginzzhjpn.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guyxjsdob.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqyeyhhh.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbiiogzyt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/grmkvpwad.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gswhpqfbd.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gcfbpwawa.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgdjasfr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdziptotm.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcobhkyok.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpbkqsjj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfskpqfhd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjrcsyu.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjcraiu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeyrmvos.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glojcfpzx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlntzbpy.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gryjjjuqd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbezdjxo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guqxambqv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gwkwxuygy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gokcbpxhn.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnuwtfbb.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gfxictrec.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghpltnzby.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glwlubmwj.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gepmfeyib.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaorktlt.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gixksebml.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprpqzaaf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjyaaggf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlxjxpo.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowuiigi.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gonlurwbr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldanvfll.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazjbrmjj.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxdutke.sHtML


<!-- 参考信息 -->