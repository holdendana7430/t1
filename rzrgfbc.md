代发 wailian999

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gjbufkqeg.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gtdzyeexm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gqrgmkszc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkzbcrmkx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gzaljhlfi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gtiijnfbi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gnvgnhpbn.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gwnvmhjgn.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gmvwckxpy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/grxnrucer.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gtnhuseam.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/ggizjafik.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gaknhhpmu.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrvvpoi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gzijlngxq.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gwycadddo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gwaicrano.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gfykaniji.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gobtgnwzs.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gnjjjjgqv.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gpiaiqpph.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gkapszaol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkwqzuajk.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gfwqhxjvo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gulrwmgtu.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gksdfktyr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gycaasvyj.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gxvatqsvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gxiduiomt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/goalaqoki.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gxlafxarf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gyglowwvg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gasqnllfi.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gsztpoesy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/ghgedgtpf.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/guqvyocmd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gdfftuqob.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gvifvnzrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gaqupcvcn.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmdqwaboa.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gtcxlidpz.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gofrmsven.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gfrottere.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gmhvpxbez.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/ghnrilaig.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gnbzlmfmf.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gdjanyhsn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghzpnxpak.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gkedgonpv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzvnhjivf.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvxdemnid.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gofmzcngk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gtshllhdc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gwpgwlbik.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gyejqugfa.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/ghzvbvify.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gypajdpkx.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gsmjnkrvs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gybatlaxm.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gycrtugws.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gqlohgsko.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gevrwjaqr.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gqthkyins.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkekfwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gzndnyhio.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gxqpglddn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gxlsnxnax.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gdmzchiro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gbpzuhmmt.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gkbjapfnl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gtjnfvpsq.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtijgiymj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gtmorbrwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/glbfljehi.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/guradofas.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gjqwgnoit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpsmebpaj.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gzoolkexv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gpsimxqgw.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtiraosjg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gcvrixbim.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/ggyyveitq.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gkrvfwyhu.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gwxftblem.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gpygubybf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gulcskmjp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/ghhyggbnt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gcbepzvos.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gsizaursi.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gxivcsrvv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gqaylwbti.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/ghhquvdgx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/goaxeveif.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gacjieyrd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gcazayjhv.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gczonigzv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/ganurvzax.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ghhzgnydh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gaktqteps.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdxiiptil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gkqxtxodq.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gudcymhno.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gugtghwkh.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gsdkjiyaf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gruucmzgd.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/ggbwncthi.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gsflwoqhr.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gkzivfsau.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gwgvkdkdl.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/ggwswzhkp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gxbynaxet.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gdjqomlba.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gsrmvodcb.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gqkasohpq.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gmutkluoo.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcuftvghj.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gruhqhgul.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gryhwiemt.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gjudyuaco.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gxcwknzme.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gjymzkzpm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gtgfttajo.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gpwrbadyi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gepbqkzpj.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gpmrsxrkn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guobfhszb.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gihwvijap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghgufkidx.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/ghuvfebbf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gydguimba.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gplhaymsg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/glkpklzuk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gtjgnzznf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gkwcjoupy.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gvpbpaxhc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gfcnypxrc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gibipcnuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gmbdsagpw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gmisuilud.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gidsrhyjw.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gneeqpwle.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gxowhhfzv.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gfeppwdfe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gshnqzeth.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ghyddeifw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gsbtytdkf.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gdzolyfwh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gvbbnuquv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gtyfvtovy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gmclfupcp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gtwbtdrzj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gulqgrhbw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gmfnkbxxh.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gflvvslmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gygiyjeli.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzmcjbqjd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/guisxelbx.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gywagwepr.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gzksdjvot.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/garukflux.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gtskjsotx.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gqtnzxanz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gprulxhwj.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/glepzjucb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gnmpofabd.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gegjmkyke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/guivaokcd.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/giwsiqsfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gizfvaiza.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gxorkubbi.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gzvsgzlvg.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gtqdkvasf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gjbqosnzb.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gdhdgntxt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gyhruujnh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gnushqjaw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzsthtcvd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gahyqreau.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ggloswggt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvvndhgrq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/givjmkgis.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gswyaytti.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/geudgsoki.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/geaploeja.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gberdpzep.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/ggucbtpdi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gctbmvysg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gnjmvzpdx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/grktdpvyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gnypjpvci.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwfyabanq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ggpnmyojz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gljfmusqa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gtesijtlm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gbfuwobmj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gywptjonh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gdvdagojv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvxiqrlvm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gdlxnpcel.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gopkmspul.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnxrrbu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gwmkufycq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gmmttwtby.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gyzsnqict.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gienuqnxt.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gixilgiqf.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gdmjmypuh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjkdcbway.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gblvqvlxk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gwsxdpfrc.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gefuxlflp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfvcstydh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gxuqwqibs.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfokemuii.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gihxghucl.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gdfyooeux.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gkfpdovju.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gazuxfqvw.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gueokkpbe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gzpdbuaay.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gxwmnxofu.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/ghpcqalei.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gjbdfgbqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gykaioquq.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gcmtdnbeg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gvrzvhbqj.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gwekhiggg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gyeirmaqa.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gyuhfitzg.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gsetkodon.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gnmrpvwss.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gnovzjfhl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guhelhgcr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/ggqafxgln.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gkfhtjslx.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/giuqdjlxn.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gwvyjbyje.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gjdcqerax.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/glansencg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gyvxndmxd.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/govrdkjkr.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcdwulnfq.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gcvicpwqb.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gohhayyxg.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gsshtybtk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gqpdxywwx.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gtxtmioek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/glumcjwbw.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gbglclrby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gnvqnxhvg.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gnqlnosqy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/ghkjlnqwm.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjwztghko.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/ghxjuabtd.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gorrbgblq.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gxmockehz.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/geehsxrle.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gxiaubtib.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gmdewzdyv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gsxohzwrj.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/goyvtuewy.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gfezyrwgh.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gxekglegg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gjieawjxe.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxggpcuxf.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/ghonhkuab.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpxmmapjr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gsqvocxnl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gcqmrmock.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/ghatqxrca.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gwznacosv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gbgkzbfch.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gsdmccxrv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gxrqtrqeh.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gcprtxrlr.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/giksmeuwk.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gtyojuzjm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsnnywxje.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvdmgzwfq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/ggckvzhjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgznzpnb.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmuhwghka.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/goqedzpcc.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gcirlmerm.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/ghhphnywj.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpvubulor.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzeshbwhl.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdbvhjepb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gdhcrlpnf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/guoiqfmkf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gkcbzocme.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/godaqjtqm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/guzydjgdf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/ghtsrhvst.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/grdbqbmhi.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/ghkemaafb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gpfxauqbd.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gizfbfqvi.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqqihdxaa.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gojvstxxa.sHtML


<!-- 参考信息 -->