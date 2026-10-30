代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gmitbuqlg.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glqvgczfl.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/getskjjqp.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gnqzxsmth.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmxtctif.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqmsmltgo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcipqdvn.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glgturzrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbrxrhyi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gtnoyjbwd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvfzyhmwe.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtjyxnle.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/grtokekac.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsixjnfkj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gsntwstog.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfnziywt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxecqqzg.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghayrckvi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokkltgmk.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gibzerrlb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcjpxpmbg.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjnjyjfbf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geosjbbyg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gblgnwnvv.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gnekkpiib.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwxtxmer.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvogjjgcg.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gweeibvko.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gaoinrbyn.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gnksensym.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltqtpqqt.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaecgeuwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypphtkvb.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbixvihd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grzmtdkde.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwtdeqp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozmyjdkk.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqmfayvpu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaztfzrrz.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlatlakj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/guiucxvcn.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpjnaol.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdvdlpk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbonzluzb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpxkikjy.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjhozrpvq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gljpvdlwj.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtjgpfyos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbqsdxel.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfuhxbgx.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gmtnsaadj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqompqrzc.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcovenrz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnrgrjzid.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ginyzcmgi.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzinznfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdbipsibp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gayecrodi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqgoelozg.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvomlsnl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjokebcl.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpkqalcc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gowcdhtat.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gclsnwvmt.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmglzwdwo.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedmqkfaz.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpyawrnqo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcienjbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfsmurdh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gnzobetyq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gphhyxjmg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjqwxocu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/grzlnotzg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafroipe.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpacnhwn.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/govidwwrw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvrrumx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grnofofal.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gspqaivjm.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjunccok.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghibqktjb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnpqccax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqijfqfmc.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/giczhajwo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gfbpnfrka.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnkojgkx.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcdclcefo.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsyunvaq.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaghoylm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxtykyxjs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gghuelsds.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjysopcvo.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gyjgqwyjv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goflswzyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwvqbsgmi.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gobjrsqps.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsmeocip.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gjgmixtfp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxehxjbug.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfymwdifk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybmyvalj.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gzktvbncv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gyzcrvhiu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gyxecnxdu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswiuanw.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwagbvtkk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjovqset.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/ggrlmwags.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gctczhvtl.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyzqmpym.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndujvaft.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/glbmyjvms.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/ggodyeido.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gabbujjox.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfbopdd.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gnecxkwmp.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzecyqvty.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjucidxv.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgcmckgx.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbounch.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/galxgurje.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmoaeck.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbldothdb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjapfisgd.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gpwjujmyf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaggfqqn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/geatsdgpw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaxiifmp.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gypcxssro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggudenksq.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhvlojpu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbanadnuk.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspyngwqp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/givheklzd.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbehuyra.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gziwychbx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwvurlq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqwuxal.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpgkemwn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtugcqenp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsteplqfr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvanuhws.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/grwhfwamn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyilpmqy.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmbzzabp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjzplsojh.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljckjtd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfgoleza.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuiovhsn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfavhzaag.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gqchrusyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoiedwer.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guvylmhiy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvmqrtvm.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gseuwjvkc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqkzjmsv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyketlkmk.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwoysvucg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrtkidmm.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjjoueyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfpdzinis.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkqnojhi.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/grzfsmyqq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gntyblatb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqhdodz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldvaiwaz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbomtfo.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwpgcac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxexaeri.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqrullpfg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gobttibuh.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwgdwykm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxiysjvcw.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grytqukpo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gnsomunsd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqlfkwlo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkujbrmtc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gffmplkhw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxvacwvp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvjmvbkas.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiddjbsm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmvfmwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrpsoxl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/getyuswkr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfruhbeq.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvooawbk.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvsqlmel.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobstpoaz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gnbtmkdho.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/glsjiidgo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevovyove.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gaqxzgssp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqhuqrq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmbacyle.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/grxxrksrh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbsgxtukt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvmaxsf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gogqqzznf.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gnbfwgvpy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfifcjnmd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpqtawjm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gwhhcngws.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrejsymm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gluefysyi.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppbelqni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpulklmp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmtnszfj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbaobuyyi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpmdysp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzqgkacu.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/geoviabos.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonaakefs.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxhmtzwo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqqepssw.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegonjlji.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqqcqux.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcnostpkx.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gesrgmbil.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwtnearg.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpwjriba.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwawoauoc.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzkbkhfhu.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gygckybgc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwwpgtrk.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcaomifo.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gszychmbl.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbijxhpq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzucjsvm.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gooxmfxzy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaaoskay.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztyzojxc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpkjmqr.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gslsaoygw.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/glpwldeku.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzhueenm.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvugitw.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gmukcmsde.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvdwjauo.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbhkofe.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkpuackd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbafrrtf.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymqoosly.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gxxevhagd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtyypvxef.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfgagzvkc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgiekmsc.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbaopfvwz.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grmydnpoo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyxyogfk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/grhxlyvkd.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/giukasdft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gockxrodx.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvseyxc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyflvczdx.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfhthyynh.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnfoasjd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsabxlcip.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gyixwjhph.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcwmobvtr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gimlbfxnh.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfektqchi.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ggmfjymhm.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gstzzaexr.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gkahzmgyp.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/godjwhwjs.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gfidzbsde.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gofvllskl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadimswvp.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gmqmnpcyp.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gevuchjog.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdlqblcqt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevtvdyp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbjxurevf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxttsyub.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gdjuwuhvo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvulynudb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaiccwqo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbibqow.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtbfnhcxm.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewbkpini.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmadarsju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftradcca.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/godkjjvri.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvoocwj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxoyavl.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggpoopthf.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gznhaeahb.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjdpirvj.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/geojvxtyt.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gjvelmdkn.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gewtraqef.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkkyjrxr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgwlnmps.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggmursudw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymatukry.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaohktrle.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gkeafyytb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbqscmem.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gzpmbqpwi.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gemylaihi.sHtML


<!-- 参考信息 -->