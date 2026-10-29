代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gjcefasvx.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gaiqwpjvh.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gwescdsmn.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gvnmgiylx.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/grfzzjpgv.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gwvwmtyux.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gjzejohay.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/griaxzeak.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gtnyujicj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ggrqmfxpe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gofadfbxn.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/geshiorau.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gqcthlibt.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gideqqpkj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gyzsikotk.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/glquahxqd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gwimpmekb.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/geygyikyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gxiykroxk.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gythomyut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gmcocxnyj.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/grdohkdbn.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gsoivadcn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/genntsgri.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxugihg.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/geroyrafy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjkkbrd.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gzxyalgda.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gvecmbdll.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/geptgrfkj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gxbebcmaz.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gqjfzgecb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gkylezqcs.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gxydlrxtn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ghewmmfhm.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gvtcljtdq.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gsczmfavn.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/glllhboxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gjfekcxvq.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gnrdwisym.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gzzhocwrj.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gtpvynyef.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gatakyjrm.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gkichaafp.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gkqbzpzcj.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ghacxmrfo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gspknrqiu.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gtizmqraw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gtupmzohc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gzkrpftpn.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gxwkkzsvs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbrgmstud.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gpbnicwhb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnodwqkde.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gqtfohgqr.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/ggtdlurgn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gqlcnlxmn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gfoseoorc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gekzirfpt.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gesbdtpwc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gzobbipxo.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gcqrchife.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gppiigbwe.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gftxaytew.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gfjcscqpx.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/genhbvrqn.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gxxzwbhcr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gyrrumlcc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gjzzbkbsl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gsvpbbazx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gqujtixga.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gxvmhnaab.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gthvfmmwx.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gtjfgkijb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gboxhzypc.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzgowjoug.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcwdwqpcd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gxecsbyky.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfpmgspxc.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gkiiajkjv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gpvjmkged.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gkukdjkuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/geqrjrbtf.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ggawfrccl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gxpwljslu.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/goftyeodz.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/ggmsejsbl.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/glvxswora.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gkgsbiffs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjtqycffe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gblszntxc.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/grtfrttrq.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gdtcbkbsl.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gwfxjuphe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggntlbvip.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghhlmfxha.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghpxmnsle.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/ggkzvyuhw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/ghfwhxwzj.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gekosnzub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gjjzwenhw.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gqxxbisvs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/grwdkjptf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gchcfimbj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gszhlahkn.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gshzutdny.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gmuuqfvkt.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gnreoxasa.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/glhasbgqm.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gxuwspxbd.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtubosqec.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ghhpgnusv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/ggrjdynhu.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gjjxtdgbe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/geccqqohm.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ggtmgdrsl.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/grtqhtehz.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gbagkvkpe.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gmnqixyix.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfeisjctv.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gkbhgccme.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gobahmhid.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvzrxquga.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gvoccnivo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/giebaevid.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/glfeyphik.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gkhnqgpfm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gffnyiuvb.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gefzltitx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbrndwtql.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/ghdkzlycf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtdvzedgx.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gsezzqodl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gybejtodk.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gzjmiaokv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gsvwomfbb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gxuvkltiu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gikklciyh.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gunefxolg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gnexyzpdc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/govgqxytq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gaemiyryg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gcsqiludb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gawlfaaaw.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gyhhigqtd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/goihljugb.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/getyuwtuh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gkkuweofp.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gldmpdgjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gaffsthwx.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gykwmamvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gycvtmyjd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gyhbppxbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gjwikpdax.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwsnfvqti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gvvfrecht.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gdblatufa.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gfaeymlht.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gwrwoawgq.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gkazxgaua.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyclvomeq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/ggmspdzan.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gxghmobrm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gepqfosxr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gjlxrfjwi.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gjawldahl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/ghdcpmyll.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gonldndrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuuclewr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/govwlnebw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gbgilhvon.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzejaqlnn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gezrxejxq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/geghvclhu.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/ghpacyeex.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/giqedrpzz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ggeglltew.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gazomkccb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/ghpiqxoll.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/grzqulisu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gorwtlqih.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxrecffwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gvhvwmdyd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtafnlyd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmpswngiw.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ghfatbcmj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gioevoaql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gmyjscduf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/grzxrlfuz.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbgdyddiy.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gmtwpehlc.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gydbzxqef.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbdkausdd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/grwtvxigk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gmeycrtzn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gflnatasd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpqhoqgoe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/goclgzjcz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gmenrmbby.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/giuzdvkyq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gmbxytikj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/guerauzuk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gsxrktvol.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gvjctodof.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gledyywxb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gjfkbbrtr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gxdpqityw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gzsmvzvgb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ggflgpfnz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gkqhcmfwc.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gpkpwgjew.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gxfcwyxuf.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gcmthnzxs.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/geubcyvmy.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/grysxzkli.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/glcosvqhw.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gudfcjjql.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gtukrtyox.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gcbclkapv.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gsjgryuvb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gamhzemal.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gtltfiklh.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gcwxqexvg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gqaxpvshp.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gyqfpahmm.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gbmmxdjyq.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/giwvxnmke.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/giteglpqy.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gozedwbfu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gifougnbx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ghhaxjwfj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjveygpog.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/ggxgliued.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/glsgbwqvm.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gswqucmxu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gwsrszllk.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gnnygxsmu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gpbtgjoja.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/guagbsejr.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gkwqckslq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gxsandpjg.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gtademsgk.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/ggrikmmup.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/ghmdktcnm.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gexvfxhcs.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/geyxszjxq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvfoiesdc.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gibjspzcz.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gpsgfqgsx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gfuvpnbmv.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gfhtwzzrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gkoqxliij.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gfsbzvdzg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gdcfwqffe.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtarsqezj.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/guqzkatct.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gbqndeonc.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gdkcdwtyg.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gcglraeji.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gijjhgxhr.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gcvdwfjxg.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gxmnhoxtk.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gvnpyvldw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/goxngdvsg.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsfclkvlu.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gdtqkmlid.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gosykkxvy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gglcxxble.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gewhbavmg.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gkwpfmvcq.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/glkntoaqc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gdevknhbz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/ghuayoqeg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gcuolvsah.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gnsisrksx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/ghlfpkxbt.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gctgifgqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gnprkkjpn.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gmuhfeevy.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/grlyupbqg.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gzwsufbog.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gvdjuimbd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvymvrxgu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/goqrtiseg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gnrvueppx.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gaykgwrfo.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grsnphtqt.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gjlimefvd.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gtojvnlfn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gmddzjymo.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gyvhoykeo.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/ghndmyvse.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gvgweixgn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/guzpkahfj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gugwdcvkr.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/glrbdkhkh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gdfiwuwty.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gmrblsopa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gyurfzoiy.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/ggzqrgled.sHtML


<!-- 参考信息 -->