代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gerkptans.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpghcxzn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gilqvumrq.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gzobykogu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gltkwqwpc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gilfmsvuw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/guejccqou.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmmfirugf.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjygspkl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geixunofe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqhrygff.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonctwts.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnldzdcj.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gujhxpywa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gatbrxawd.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbblijuzd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gulhwnrud.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpenrwat.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzcdcmwtw.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gyidxrckd.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/glwoepere.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqrnktfi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzennyzou.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gbsauropw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnicbxehk.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhlrvghr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucxgjnrt.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gyituumzo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxclzneh.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/guoixqbdb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgusrnp.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlpjyfse.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gijscurfz.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcplxrbz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvuuzsvg.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giewimzup.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gchpwlbcx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmoizuoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbriiuwx.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/guklciswr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grievepgp.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvxxisxxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbxlewvu.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtkysehlc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvhkvnowx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkfczwzd.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gvdwtfism.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhdjxpu.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuzzfvbk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvmxsmgbr.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxmlstql.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gszvmvzdq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafrblbot.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsihkoxbb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gktxoxcox.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoelqwvx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhidbtyu.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gyzlgxnzg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtannxy.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvghpxnj.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkydgykg.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdcoztxz.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gtdzjbrbh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcieklur.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gwiozsdny.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgsnkbky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gvkouvyse.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gljhcjypj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdblxpi.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gstnsxfks.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdkrfujy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/giragafsm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glxwypcdm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnthzozhw.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gngpliiaf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtayyov.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlryrvmv.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gartdrpag.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ghlsfvjjr.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdwveazp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfauvhrnl.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzwxnvfu.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfoiqnqf.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gutzyjgqo.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxlekfrr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbkahewrs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnezcyhla.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxwgviedo.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsollywr.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvufxknzz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapftfkwe.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gacehkrmn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwkttzku.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjulidob.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gkwxhqswi.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdtuymvir.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvtobmqq.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gjfrvidek.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdshlop.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gemvnddnu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvskgaj.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gteszxvau.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdfndqc.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwtpspsey.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmffffzow.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ginhtyvoa.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvvqeltmk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwvwugcvm.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gokaxcmxd.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghwtryrkm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaczixhqc.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gstbreggv.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gemvfgjzh.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxuxdqtgs.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/glllvrkbt.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpcxoqrcf.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrktifa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnspixeds.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlgjwxp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gqenltmnt.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/graltowhj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqbjkfbh.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gccjtalkz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvassnime.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggjbxmcej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbijmcgim.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gajimotii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmrmcygw.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gyronjane.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbnwvcrch.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvdlkghx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmfyzvdy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmejplo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvcflwhh.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyluexsif.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoczjzja.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbipbzuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gqfouzhyy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghrmdwjpp.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gegueyrxm.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxmhxle.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwsmpbzo.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/geerifetq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/glkfsnvoy.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyqzjqus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrpniend.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gavyzayal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gevpirsss.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqeaezx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqurscsqk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwzvyydd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gioigbqkj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbzrilex.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhtlhbew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeftsbkp.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmrpeed.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/grvmtvret.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmgtkhbz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutabjeft.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gwmaswysh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzfqtgwd.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gcxqnbplu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gedkdvler.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdnjabx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvdmpfsvh.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxnzjlkb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkpyygqt.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdsymjtd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwpjgtqxl.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjcynatf.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgqasbbg.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gubojznmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gcuaitfjs.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmohsyrbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqihvmgx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrwzvxg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gniomxpiq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/graebfjvm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyccfqzrr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoyajqsw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gygqlmsry.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gquttqaig.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbnsetllq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtixrxdu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/govimvame.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/greyrbisa.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gcioexmcs.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvofxaxpn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfbgvtpep.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrchoob.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdxkbdzf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgdhhyh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgkxfqmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/grukzosnd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaskqaeyb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ggruzwyjm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsszlvkm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzxwrsql.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzptbtksr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/glyglklmz.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gfcpbcstj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gblmcoyfl.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhhlvusd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmrfgtbz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcbsacif.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsigxxiwc.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/goufitalk.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkmygxlo.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmwryqv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwerhoeg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbjtumohd.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpizteuzg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/guhlpkkia.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glhbjkjee.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxsnwjbv.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacpoymso.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmibauidc.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitjmumi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrtwrnnc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyojzbrn.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlsunnkt.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjckpnbje.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gmflbvqxk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/glowhwygj.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwwbkhc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyszkuaof.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gsnekgifc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwdahdz.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gstphmuap.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwqzulqp.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gmlljzbjs.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilvhkjgf.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gglzuvdbx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gpikfchrz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggczshmbq.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqapvpnft.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/guofbzyhb.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrguvvdi.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkcciyps.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdycoxret.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gurqsssal.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grikwrmcp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubssxdr.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gldcopiuy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaoqdtyq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gplskkdwi.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpgxknjv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gooykmdrb.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gmmskrjby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmptgueej.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhiumjij.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gzoaxfsin.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/ggldfbqzg.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmtugltwl.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/guqopvlhx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvemtvya.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdcvmkd.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsjsovwf.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsnnlpnv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvpivuc.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcupahwx.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggirwlscq.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gongblqob.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqhxjif.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtodwju.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwivtwywp.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpigfcvd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhzdnufy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmdxszzn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzuopvlg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsxjzztr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grauyogcf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/glxqaljff.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcvypxvi.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsueswsm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpqnhprv.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqyeodatn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlrkobkl.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnvyovadl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gworsaqqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbciwgmcq.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkqsireuc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gnsffppzi.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gehawfoob.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkjvfisp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gomrpvjfj.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdojwgexq.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gkkrrukmd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrnoqgn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gyvbrxhmb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaknmiywi.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhdwsxi.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gptdpcbjj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpipzrzr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhzzutn.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gelvsnzed.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gctrqamzn.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gprinveih.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcylewhu.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbdkfjc.sHtML


<!-- 参考信息 -->