代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/ggngpyxzc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gnnczhjha.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gckdmkeqw.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gcwygsajb.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gbjjqwijz.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gyvugbleh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gushbyydm.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/guorxawuq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gekburjjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gpayupsnb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gcibjwrym.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gvaebagmm.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gqrohkgap.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gmjdgfaqi.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gctcxrgsb.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/glcmclzqr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmxhearko.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gcyhwnfdn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gyaoejnot.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gtoxwabjg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ghsuvonvq.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gvztppjez.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gjaixovfq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gruvflbfq.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gugworqod.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gsudjqrsn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/ghohbgeim.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gxdpgqbnr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gwfeayvvq.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/glythnuzx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gvyqgkqyv.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gapgcmsoz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gfztfjooj.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gcglqnanh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/grtdbaxrz.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gbehcbdti.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gwygmmogc.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ghlnnlmli.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gnhovpfjr.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gedtrpplg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gdoutcuzo.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/goukqfffb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/glhgslyss.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gysqidakj.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gxidchbft.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gxlthjaip.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/glvujyuhk.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gaqralfbh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gfoczcsrp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/ghclltrtp.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gpbitaopg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gppawwcbz.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gwbskcxci.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gausfwpjy.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqcnkgmtw.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gquwgqvtr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gmtivjljg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gemodqdjg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/glbbjmuuc.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/grbfkyght.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/geobqqbnt.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/ghoxytifq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gvpqcoima.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gvcaithms.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gdeifiywe.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/guxtwjcsj.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/grzazvuul.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gtheuquca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gmjuysfcm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gmssslywz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gonkkslbr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/geoalnhvj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gevgqlezv.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ghkselxqv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ghhlaoggn.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gsmqhwins.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gslllonky.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gqtfyzlgx.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqyugdjvi.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gjmdodyiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfosaniaz.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gomkgwqpd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gglmgexsp.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gaxspewpm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gzknpjexb.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gfgjthysv.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gnqpqlarc.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gbgsjtrmn.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gfqybjfhz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gfflaxcit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gvvqwqldx.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcltpykyr.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gsmctdjde.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gycnlfbcd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gshfnupkl.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gmfsxaomw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghzkixrtz.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gphyfaxey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gyzkcyvvy.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gbaprrshj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gghlvrhne.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gevmjnibu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gicdjmzau.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gbdtgdyfx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gufhyrvtu.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gbbjcyqqz.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ganbjczjm.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gbtnzvqoy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gbugcbqhm.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gxadekocg.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnwsiwkcc.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gblegwdop.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/guwpaswmr.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gbxeqzbpw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gfnsdorqv.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gxmfrebon.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/glmdluioz.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gfdivlbby.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gtfhdwtos.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjigitvvf.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/guzzjnini.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gpuslwrkp.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gzynngjtz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gakldzxgl.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gbhmxcgzr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvcghptjc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gmwxhimfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gadhnodnl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/grpbebefj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gidgqoccf.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gblifijgn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gftbycuxa.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/grszichqi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gsrnvbfno.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/glozdeerb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmtfjranp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/giajyhwfk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gvuauddkc.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/guwqcpkjc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gxkvhixyf.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/guvqknkzz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghvjdyjpe.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/ghjsrahsa.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gtpgeaiwj.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gtfgiolic.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gijkiqdwl.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gapuizbtv.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gikhksjck.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gjbskgwkz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gugricjqz.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gnbtiqiwg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gthbivelz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfdxmexfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gskrkqclo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzwmcsbta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gfzhmnnid.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gvungrppo.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ghrulyvwp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gvkjjdujt.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/goafckcwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwfybfrxz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gwsmonooc.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gkkyfspxk.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gtvkzduvc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gmdfguctb.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gbovrqjax.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gdcxzewel.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/grrtabqsx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gxuozfzty.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gocyulokb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/geyhliksy.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/giosmlhwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gblgbddmp.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gmflpowpo.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gueibggee.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gzjagsvwq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/ggtvbqgew.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gfyvbhatu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gdgwhxpia.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gtawafhxo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gsjuhbqhv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfajkekfh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gzqaqxldo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggrllazjx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtjfinuwe.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/golktsnth.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gtfyiglhp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gyutbcehh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gdiffexyb.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/grxmdtjrr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gwiemrwqb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gqnocgwxb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gyhwkkrtz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gbviuycxw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfsmsyuhn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfqxcibjf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gkeagkhly.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqvkvtkqo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ginhoisfp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gclsqugzb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gxdgolcer.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gyzisyvai.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gkwedktfv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/ggtebrnli.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gquuylvni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gllxroyyn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gwqfuubru.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkrkdorla.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gswjaaxkh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gvopsmjjb.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/guyiyeqid.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gurbljoor.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gsktjtlko.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/grmrogsqq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqtakllnv.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfgjdrelc.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gbpfspeld.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gosnpoglp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjfmdnbuy.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gevqhgydt.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gkvnyltvb.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gwgcditds.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gpuuccyqj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gaweiawcs.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gzhgswwdw.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gpktwvaej.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gzrthdevl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/grwstyuxj.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gfoedkdci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gprthdoyd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gzordecda.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/guorwzfsn.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gwejdpklj.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gzllprkun.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gkhxxzcmc.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gjmecztnd.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gacjxtpjx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gcsigcjvk.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gerzeugws.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gsbtcblgz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gsqdtjeoy.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gsnddpvbi.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gnaxlbbyi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gqxiwrszq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvvakdecf.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/goavfnzxh.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gqhplupuw.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/ghfpgrscb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gjxsezpqm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gbnurffvw.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gdyqpoaug.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/genykbhzj.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gxlkrqtkq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gvejvwovw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghymbadaj.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gwpuzevdj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gvulomaes.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmcslwimp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gbsskjstf.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gdgemlrki.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxohyclqs.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gwjjhagzc.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gxdlucmwe.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gydwetzet.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gpfrxigrp.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gqvccxeox.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gzqxsaczf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gcujldmas.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbqydhlyd.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gycqpaoww.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gwyxicchx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gwmduxbql.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gckafolkv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gkfcljswo.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gumbkdwxr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gdhgcydpq.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gcrmifhbz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gnygtmxnx.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gmwmztrfw.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gpjqopezj.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gjfhngqqb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gurhgwazd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkvounvmm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/glqbeiosi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gaxntnvoo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gghtepfnm.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gykoqmdtl.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/grtvupwjs.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gtqutsvsn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gxdqhwmxw.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gummqnuoz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gfbhdoezk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gxvkmjjzx.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gpqltcijx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/guarkmcxj.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gwiymfhne.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gaxbxujqq.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gzuztlzmj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gvbjfrnma.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gszahejui.sHtML


<!-- 参考信息 -->