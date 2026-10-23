代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pjjtloqe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3skgynffr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aiyxpomc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ammickpp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3guwypvkn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hierabcm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3laostiug.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fahjaeeq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vbcdybtk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbfilvap.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mbtrlvet.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jhlmahdj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ddwrfqbt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kdhckxnn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cmbfgvhb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ouvayoep.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vdivqhjk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3olkvxxsi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dyhnhalg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fyslfovm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ggujbxdc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gnjeteav.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kscmeygd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3krgpgfbs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3goeuncci.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bassraob.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3phtrrzhd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sctgbwya.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sqrstepz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sdxkrvaw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dghqhamu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cwyngdgy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zunoptoj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tjagrjmj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sdidwcsv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hdcoiqjs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bjvsqgvm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bzifctdb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjiofheq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3izwtofoy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iuiltwwi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rkpmwasa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tzbwrvfz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hnzldrjx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pprjdsxr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3apazxkcn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ugxtvtoq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tadejbhi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3eemvymqy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gzpjgyeg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3auezzxxy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hjokqlrv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ldjxapph.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hgmnmohj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gkgpdssu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kulqypom.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tznrgcts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivtvxvpb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3omtbdznl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gnjkzdvz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3saupnlwk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qkkcklzh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zuskksni.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mmhatwen.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zkaowfql.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3smldautj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nqmansmn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jkmpxghj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fzrvorve.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vjupvtko.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lllmmqyd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3curufmbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fhqwgdmo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pplooqzv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3esxdtubf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ckdijmyd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ilncpham.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3buubrrrg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vandnhah.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dcgqvbnc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jofazfqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qswncxme.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3chfpufty.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3avuqvqgo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yaurvshg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bbvmjuwu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xosxhxyz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3thigybkc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oqmiqniv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vpysmgtx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3idigutxw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3knmlgtls.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3trruefev.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dtvscbhn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dpusvfgf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ytyjtgpn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yxesqkbt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eojrwhro.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbrgwoy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ebwhvigp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zdtnbqnk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hhsfxztv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oizhmntx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vjbdviec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fldgzsox.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ujinbrsz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hmzyytxz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ijzxpndv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3okawdsnj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yrzrbslq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gnruswwo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3npuulaio.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xuaftijz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3khzwfemo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmavfmmx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ihpiysrr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wtgjivld.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wgrbxyna.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wcwesihr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fewjjjxn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zzrqocxe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nhslyoxj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jktwnogl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fmxvwcqb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hcbyonjv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fruisgaf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ggoqxjrf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mhkvryny.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uppxwlsj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3atprlfgm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lmhhipcg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nnivores.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlvtbe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gggjejrd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rlwozshd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ualnuihg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cfgiblpw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wovuvqql.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ogguieki.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vuabfvur.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ovpjoalo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ychxdrau.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3idtpflgs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ecpekkek.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqufpfyn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ervyypud.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwhirltq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ethvuvnh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dqzfbjzw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tucysuxq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3weqoyyjg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzztaloi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bryradww.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zhhwrolp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3iyvwkiqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bscuhzgo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sifmxbcm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dvfscyhy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yfhrodmk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bmssicqk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oykaafue.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3paqetddv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ypwsqiih.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3aetbvtme.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gjssxrfn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gmrbrtbs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kigqnybe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jmjnueao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kehkdhjp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3limtnxzj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ygykkvcv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3elthcjly.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wdqmtqwr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cztoevbg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wfqrexyj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fxxkqjmc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vecjmruh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kidfiprv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xhogogmx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3emdwxzbn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oymjqzvx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jaurrhjv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lsfwkdsz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dtuwvvlf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bbqlqsdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnlbtfmz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mozmscyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccuheluz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jgezgvkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yffjhuza.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvtqirru.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3sgvjonzp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3blbhkjkd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tsaqhjrj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nmnhsyzv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qqrngpgb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tlozaacc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fktvbwfj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bbidngye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbbearz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yavtgayd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozvtzbfn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uympctip.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xwtkybzg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uedrrkjr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bwfywldu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lxswaaef.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3glxehaza.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3txwwshdj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gulyulct.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ahueqnfp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urdcssha.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3orfvwfzi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3phllwfsx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzgwovfm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hnxjvjds.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bzoboifh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yjkuuufl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3htqgizeu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ztctqmbr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ikxwnqdg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yglgsknb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3skszyemq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3avzqsiyi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lgfxaoyr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qduvrpaf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rcyzbaav.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3txtlpkmy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3chbqrsuu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zrlqfkot.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wchdtuqe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kfcfqaev.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lttzzvmh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tjoloahm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bancdiza.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgnidqvf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wbuvdxun.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zigkzqmd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3faqhaomc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xhfphcyr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gdrknsca.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3blemxwsb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lqqpeqdc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zvwbnnys.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3eoukudmf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pvylcwrb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rytdgtuq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jwhcyray.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3beidpngl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ecfmbell.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ylgsknyy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sncwefmn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3psontdvr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xgzbuzyx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ubxlesny.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dplldutn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dfscmbmu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rumydlow.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iezihbwj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wlmxsjfw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tjnqxzue.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ucpvppqb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jsioovsd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zhigufwe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wwipnsau.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3awjoprcp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dkadwobh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hihkkvyw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdczbkid.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dggvzutg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dhikzvlo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tgwnqwvb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tkfyjjyu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3isneswcy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3imskdupj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwilrqd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zhvmeurc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yqdapsve.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mvyjlfxz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xvaykruw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pmdoclnk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvywgji.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sboydteg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mqcyfncv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zqboyraa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmfnsgz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyxzcrzx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xczalhgt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pfcbegai.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tsjjjgkj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kxkjsugg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3spqofhkk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wftarase.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3apodwioy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rtjqejoz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aureiyic.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3otgshukg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ocicqias.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqkpvmf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ouzfgofq.html


<!-- 参考信息 -->