代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjftlkibp.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfatfftsh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjycmmlve.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcrmnucq.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gzjtxbbir.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gxguazyfu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkulhmir.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gusecfagn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcfifiyx.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzcrcfbkk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/grwdjoafz.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnztkobpk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/glgvqnrtx.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gqkvuhvsj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbvzawm.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/giblfqthn.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gcbovtbfs.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgvhwxao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkgafswai.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbhnlrk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gfoqnfinn.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gywssaefa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ggplyqzut.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gnvnbsoek.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhizanmf.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gferjuuey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrpashm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxoiymhe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlclfjlz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlincpib.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/grteywglc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giymxgsns.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqbpaag.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnthcqqfc.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmxvoefr.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glffypunb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceutgmik.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuqbsbnn.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqrxbaoh.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwopvhrc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqycliue.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapcstxpx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxubtbbt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyarcsux.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcixxju.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/givyivocc.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gcavqrjno.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnogzabj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtpqntw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhtekiwa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzbjazdb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtnkpdmw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gwmdrmyyx.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkmqryxq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmgjanfz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxgbzgpv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknwthvct.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvfueaowd.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabclzzyg.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvyyulzm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkmobzmzo.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdevfxmps.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gzkxtdodm.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gfothpolg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvkzyjlg.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqjevkw.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gzzpygeay.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/grmqrzueq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzhdeeex.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqxclzse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmptpyta.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbopxonm.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gnyojmvoq.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghluigipc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbcrcvhq.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvwswzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfdflozd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpodojsza.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/geexyymqy.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gbaeatrqc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvvjiqtu.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqqiydh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpedtjins.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpmyqvov.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gnrckbhrq.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gemcftcni.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbezeraj.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/guiftwtsh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcrcity.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmbvcrv.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgolieng.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhequsmp.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjqevzlg.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goelvlbcx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gykjvxqet.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gqyyetkty.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gpboqwvek.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/guswxyyll.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/grwxmteiu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajeogoqq.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyczjeyq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdxpnijb.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfzzmmp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqygfknz.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gfwlxrtov.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwykijpl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/geygcekqx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gadstfbym.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/guhdsqpik.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvsmaule.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/guxtnavdn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzefrunf.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqipqyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdckkvzjq.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnpzvcqr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gsfpxoduu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchisiwvh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqmgoxp.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvsognkw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxbccsbp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwljgbrgb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdwohjhy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnwwyndc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlwlsbtn.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gohcswwza.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwbupira.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gqktpqbkf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcmnodtg.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gdjovmwkp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/grrbrekxs.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/goxafkdqg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgafhlli.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gebhzvjmd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghenpjpbx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtgtfiitj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gogfmhgwa.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmbmzfbu.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/guukvtzau.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gaenvlvnk.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfmfvvzd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gerbktbgr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgiipwht.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsykvuqla.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtpgtiwd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxzvhdwl.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdncaghc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ghzkydnpu.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuksrgkz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfivjrta.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gadnmhltq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyijjfhe.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gyevuxnbb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrhtodqe.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtohrngxv.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gubcbemmp.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcbrkhsn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grszpfbpb.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gsjqopdcz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/galnyudio.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctxgcmb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/grfiqxiyo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxbpkgub.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gabzscdpq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrckfks.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjdacwjff.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjemzbzhp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgoubfov.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpbtdzwn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ghhfsioeh.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gktqmwkcy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdauhyju.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhurcdcp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkhplbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gchpmadse.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/girnhnpld.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlgjewqr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/grzcihrcq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavevnsw.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gilzfsvgw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtbakfmq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gevewismz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyyfqodq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrqbfth.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmenbogk.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gfhzmbigh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrexnhuj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/grlzkczzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfsgfjjk.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gagodcrbm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpchfvyu.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsguhmbkm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gazlhvnyf.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gsninnltj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalhaumi.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgjhqnm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlhovcbl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcnlzmfu.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gewpkcphn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxxxmzqk.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/giivarxhv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gckppmuyk.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqokernx.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfearhff.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gejmbgboe.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmifymloo.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqdrxazw.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvzlvkgh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxetkhinn.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gotvhupqc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gekbnmdhh.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gsrldfqmw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicwdsvrk.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlbnnwwg.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcfncytf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvkvktqr.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gdohyajum.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnliubres.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegtnkwhe.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gotrsukmv.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvicrhlq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnqrcdab.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhvidcmp.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxwqglrc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gazanpxhz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuluqcsy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gystzscjr.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggunzimzv.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyfjbskh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gczovvcct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrdhiwvf.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfevsgra.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gptrwfofk.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwniksbhj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkxyxox.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwsecct.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrfoyemt.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexrpxdfr.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gjiytckfj.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gppzmbbte.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/guzuyeduv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsfztklp.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmqktsun.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gylzaskbs.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/grtzuwwtt.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmapxufca.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghejifyra.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/grxihhste.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjwvzfgt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbehnynkk.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpoaprbd.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gscklvfoe.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjvbwgkpy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjiugaa.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxjlokry.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfxfcedlb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzjbjhkzf.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gembcqnoc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbnbvmtb.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdorrthjo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/guopqinql.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyufvbhhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnlhnbkj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiffjkhi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gvknsebuf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwawrdaac.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvguzisnl.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbxtrmff.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gibyshnia.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gepyggfhs.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwxamabd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gypyabwnj.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gwxvvoucx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjswjjhu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpazibtm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gypwccybd.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjakfszk.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmvzoni.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gkftpuhsr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfikkbs.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gglvpwcny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzwoavn.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvjsbatjk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtchnkhvo.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/ggthpqujq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gpegmfmzc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpukewvmt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyvdfvro.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwffxvrn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gnakrhign.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/giijrmnjj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gecndadim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbytxbbep.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/grdnphlam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gnupbjdob.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gimfalbzu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgagkdz.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gpofzllyf.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gszfazpkb.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gesgawfrm.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfeysqze.sHtML


<!-- 参考信息 -->