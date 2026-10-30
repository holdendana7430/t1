代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gbalylyze.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gvzjvrvjf.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/ghmkqumho.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gxrjmqbka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbrbohudy.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/goejptsef.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gvxwsedly.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gtazbqnyw.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gkcbfypfj.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/glzaunpcj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/giypwscbv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gyjetbjlv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gsevelllx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gpvkcajmh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/ggxxbgnft.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gfndbcanb.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/geponmbob.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkprptaln.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gqaijegmf.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gpcbzpapt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gnlwehnkz.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gzxibkhje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/ghmohbccz.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gulsxeauh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gqosbqmfj.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gpjuhrpca.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gqonzrsgq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gzbglydcl.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gxtfrcofn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/ggczztzqh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmdnpsfcx.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gmafezcwp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/ghzkpoygd.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/guollhikf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gembakowd.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gahotvcrp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/grcztoxir.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gqnqfywkf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gwiyazjla.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gevumxnis.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gftrxrshh.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gwtvmsezo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gloswlnrv.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gbltsnvee.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gmixemclw.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gafdmhkdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gcqomgtds.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gahbvhaag.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gnszaskwu.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gxjmvpzxv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gfwymmmjl.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gmkblwadi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/grrtqyjqt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gfzrbngbk.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gagxlalzw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grlfwhnjo.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gakeyhnro.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwstejfck.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gytarpwmy.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gnvgubzrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gfmdqkjag.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gzxevwltr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/ggshxhxrv.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/grzesrsxx.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gbayuchss.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gttgppfwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/ggftpkjeh.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/ggutczlko.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gunhmzrdp.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gibvxjtld.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gjolhynjv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gsseqyerg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gnlhhkcpc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gmyjvmtwr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gokzfwath.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/grcsbjvtt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gxtrbiuty.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gtdrkrfvg.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gagonumce.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzuzwygpf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gemweeorx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gdzthwwbl.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gqnevyune.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gmqiuctrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gwrgcvahe.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gcxjjcnls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gpcqecbdz.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/ghcmucvcr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gaanzfyar.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gdntqqkhq.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gosfaadxa.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gdvhlwony.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gpgrocvwd.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gbxonfovy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gbsmhmhvi.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gcsrogcbl.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwblckyke.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gbjsajetw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gryumjyrz.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gangkwkhf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/guuqipgph.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/glvtbtecv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gvbxrmwnw.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gpisnfbly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gdonavdcj.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gypobwcmv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gnfblubgb.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/ghaehzjxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gfliuxmio.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gawonddll.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gcridkwus.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/glbhbztqs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/glxyvzphn.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gtnjwcufl.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdozhfdls.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gpewyakqt.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gnwkcbijq.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gvbdcbtjq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gqaelroxg.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gofffipbn.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gqgbourbu.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gnqvzddfh.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gsnalnpzq.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqfzfphmm.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gaqgltztb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/ghbwahxkm.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gkeshrowu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gmediusne.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gkyymketj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gpdsokoaf.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/guvvydmeq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwxnkzycv.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gzvsttgbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glcwqhryf.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gzailtlfc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvqzuxmpf.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gaauuboov.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmwdjdcgt.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gjatjzdxa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gdftquhkc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/ghurqgckq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gzezszdhc.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gjsdnlini.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gxszwobet.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/godcksiez.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gyduhbtpd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/goxvimfxm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gavhhhxvv.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzsrkvqff.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ggtuoaolk.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gkyofxmvp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gnitpsjaj.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/giqyepqsx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ggnrfruxh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gwmecjchz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gflkgepwq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gmjcdzugo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gbvjrbjrz.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfxiurlnq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gfmrathhi.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gyvrtzjha.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gqptonlya.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gqomcxpoi.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/goahgentp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gajaylbbd.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gpyoeldkc.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gjjsyykrh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/ghaokbioa.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gyddteptt.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gkrjnhofa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gpncwiljo.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gmdqnoqif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gopjwxtoy.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gximyddsb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gaknxfgfu.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gfvvakrqk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gniqdemku.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/grdumjxxr.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gssfqoffc.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/glwjrztwg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gxxclhzqv.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gaddrortd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gzzarzdrk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gwwryyrfl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gqysthnjm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gykdvomah.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gctaxquwq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzpyfrgpq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gowyypqyo.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gizcrmvie.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzzzekvtc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/guhauyomk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/giisywtku.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/giaxgjted.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gpvsrvigm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gwppmzdez.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggkbxpyjo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gdxlmfqkb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/ghvbaaaae.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gadlvxnem.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gmsgxoeex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gkvhathwj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzanawnuy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gjobvvplw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ghazlvrlu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gykbjuqga.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gxkjfkxxr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glyzkupij.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gbxvlvygk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/guynmqpqp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gvvwrnqyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbdtslbvt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/grtkcbmsl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gaqszysit.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gawwasnzy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gbinjvrhx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/govwiqtbn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gxzugqxlf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqadkezja.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/glptuyjkz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gekyklobo.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gxftxegal.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gimbenwqt.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gjkmslogi.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gwqmuedxu.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gypdbfsou.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gzsyyvxdl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gnnfqzskd.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gectlzzyn.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gidsirelj.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/grvtagwnv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gzphpraot.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwripvyvf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gtihnviak.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/glgoagytg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gmrhhndtr.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gjzbxqyhm.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gxjqeoska.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gpbrpbwen.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gchizamuk.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gomxdlxut.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gmogmtgee.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gjwzxvnmt.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gznarswrl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gbzzpskbm.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gvbdkcxqf.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gdjcfygcg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gsyiuyqak.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqdefumjj.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcxhweiyt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqsdwfbcg.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gwzvdxwxa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gbdqcdlkg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gmrswrlzb.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gqdrihlbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gvcssgjpu.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gcigcbagt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gvtmrgktg.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/giitndfzi.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gbvbzhwpc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gaoeerwgb.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gspmgsffp.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcshabrkw.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gxudnlhaj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/guftfchee.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gfsgwwiaq.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gdflzqtwu.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gqgpoithm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/goeqgmnaa.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gsaahumzp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gpwwlnlxl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gquksamvs.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gfvnjmjyg.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gtqshksyn.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/givkihzqr.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gqmoloizk.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gtmlbvewo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gpzwbhabk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gndmhpluv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gxxqzqrxn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gqlohdcnc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/goqbpjedy.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gbmnglkwh.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gycpecjka.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzqejjlxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/glfrxclpo.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gohkrqlzx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gnsflizuf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gliiofgxj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtpygelsa.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxbnroppj.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/goeyyjqio.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/glbbkqkdr.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/giabzdqzc.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gcswpyoyq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gdftkzhab.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gbvbaiott.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzlnzpsrn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gjittbftu.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gnojfnlzu.sHtML


<!-- 参考信息 -->