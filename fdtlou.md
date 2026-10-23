代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ortvdgpd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3itsaelfk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qnwjpcyn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fuvuuijx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zifleczn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ygixrljs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3apgbhsjy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3muceuikj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rbylosny.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sugmrbcz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hzrfbuxl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qkzhutpy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3imnnkcyx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3eapjcwrb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3euolekeq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3akinopds.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vrnyvvsh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3loiwpjmq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pmdbujgh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3reguyvti.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3djvsfcir.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pgqplmrs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kxyghvtm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dvjghnuw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3otbhqevo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nllynkbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yeewaely.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zsivioub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ovzumdfh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uahtskan.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yzrepjvp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qchtyohe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cgrsgjkt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ywyjcqrw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nztqiqaw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hntdmviy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ynuiizzh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jxxxlxam.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gsvwoxku.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dstjwvrg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3iipludya.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fmbskchs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ukpkmlys.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rrukmgji.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hcvwtsvm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xhgbmmpj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3peadcicv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tmqqipdi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cuoijxzs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tesrogxj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3irhkblbk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kofbczmc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gdnvjdzx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eowryikr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3togixtep.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3spfbvsbl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3czemlgfs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bzeoasho.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qzgfafyy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgvmrfoe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hyxbbfae.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssohapkg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dojqobuj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ffhzrnga.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kimqfjyh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eoodtzdi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dyylwqpz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hincsniz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3syksgbto.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bnqhyntr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3uvvxfvkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irsumjhc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zxbdkzhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rifeysrh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnbpnlsj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oerplzgy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vtwvhehd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fsknphwu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jkcualki.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xnzfvvnq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lcdtfdsb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3illyxpkw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jucbzsmw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3snaadlqg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwznrmdg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ivokiuid.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uhditrff.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3slasynbf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fmwdiaox.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mfnuieeu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wwpppgag.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ywqocvue.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ikhlocqw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3itujbaga.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3slwxyjhd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qjpnyexe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uwdafyop.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wuikarpl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gfjixzqm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wufoiclh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3evsrxlaj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3waxiwrem.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cwlrpijx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fszcdhsn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3szkabyol.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fusixjvf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mwsbyhiz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vmymoukp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eueechgh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udonkzig.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bmuzkppf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wjwnmxqg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tkvywpba.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3elfujroq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqlyvwgi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kvezekms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xcryrrfe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzgtdhad.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dsgncnif.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lsoylnnl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3goyurrue.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wjhghxgc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3spfjsmrc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jsmlvqar.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bfhltyxx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zjgqulei.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfedmfq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fuccpwnm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3repgxkzm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vynlqjrh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exorgwpm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3incvozub.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gwefnudy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfdyzwin.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3davpchwa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ezkrcesq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3sgrxpoqh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xvigqmdx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lldfohms.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wfctmwxu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sotbhomi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gxiwacvx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxbylkpg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3oycqhlir.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3smboemiz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dbqhvpfs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rqiiiycd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpkmmown.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vgzbzevh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pamrhchy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3akbcdrbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gljqfvwl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sbcegiqm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nospmsgc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xiafvekj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mnufbpsh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kdcuqjma.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bolkatgl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kzvkhlin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gszltise.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3deskteda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xncozgfg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eaupaxnu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3afuhvrvh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3trxbpixx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nmqkwail.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mtlzntdn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3acucvzri.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ojppbybz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwnspgkg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3oojmcwxq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdxbtgba.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hbykgket.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zfwdrzyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwhcoijl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3evhkisax.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cjufwdgz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jhwtwutm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bqktepby.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxplsj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rldixief.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lixokgdw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lperjoss.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qedsoqoc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pamjqvrd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yvektmwb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zluulyju.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cofrwhlb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cdxwdyiy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fnbezbek.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3peadhmov.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3iarujcpv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lttbnzji.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3edkgwgci.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fbdnxphy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3noqooscl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvamonwm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ojnwyaei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3twyhesas.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hsepyggt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ukfdrvtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otdhdaam.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3geyiasnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxarlhqb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vommlngf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hqtgfonf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlzvghco.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ghjmuvsr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nokwmwbb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jfboyxww.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dmjimzld.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvhpvdhg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3odawzogo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ziamtvti.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3icgnasyj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvrnccn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dpamflbu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tstxzlcr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ufemckxz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3erqernxk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lnumhhwx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fkikzbyb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fadjibdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qbrwqfba.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kgdeustt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vmgrulgq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bmirvodg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3knxwyqto.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3owyqjawa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yseluzak.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mnyyvfbn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwlkqon.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3glufphhj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fybgwsac.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsmeesmm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mffuzoob.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3iwpfpecq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iykkzngx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lukugorm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jicaslpe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3krxfjdah.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3fjzrmcyf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wrcjxgps.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cxprrygj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xwndxvgr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qtqkkjzp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ghcvftvi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3siucgpgl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cnytqrcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lghtvagx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uafvktep.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3swchtsmi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hktazuft.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3sltmywhv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zobijjuo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tannhaiy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lolcioru.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jecdgemp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wrwpbryk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ycwrsnws.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kzvtdpdn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dwlwfyle.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mgcwhmpv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sfkgvhow.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rcprximy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mohyucaq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmqzvmvi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkgvgdud.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gyoautxi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qeonvkwd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jqwhsyzk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3udlwtzji.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nwtgrzkx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mzlkizee.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbnlrxwc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qkjcllwy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pcqhjbga.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gqpslbrt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3sdcidoqc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gatiugha.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3htixkeii.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ltxcjogl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3chteuvyh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xpzpddsi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljcgcrkn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uokedacs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3clnoezuf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dldzvchb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ffrfoybd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mcnroyzt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dadjycbe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jovynujp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vakhuoyt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkqrexhl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eywkqslf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyealjsn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gnhvwfsa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3avpjhiqp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jxisbyxu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bjkickrk.html


<!-- 参考信息 -->