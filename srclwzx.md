代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gxcefxtrm.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gmglujvan.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gqcfolpmp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gyknnaimp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gsfdmxxsz.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gobeiiapy.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gewktzztm.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gazmxrdsk.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gqceqglgd.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gnryexrjf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gohdpxbgl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/glfxwcbdi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gjqzpfpcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gqsjnnvnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gylykslkg.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gbwcojahi.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gfktvmzpp.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gbkuwniwp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gxwfbkhhx.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gcdbnbpfs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gvrajkssm.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gmceqqozf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gtqoyfiiz.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gukhmojtj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gypdifeud.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gpmcknlah.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gmrzsupxn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gpyiknvsm.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gragzntkp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gaureyapt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/glcgjpfsb.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gjpazqjrn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzrrvzyma.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gpaiezwun.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gwahssmdg.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gumwllloq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gmlzjqswu.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gavzmmzty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gibzsexde.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ghxgzhbhh.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gffhnfrbi.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gkbsjjssb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ghuzupbqx.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gkrgcwnjy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gmmbwvhkj.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gptpsodtd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/grqmkgtbr.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/ggqyzvkwi.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gmijmzwim.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gcklvqndz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gjodtxopv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gkauvcpyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/ghdovxnyi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gleiqpkws.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/grqckvngb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gowvrgdzc.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gqdbxyhtr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtkaojtzn.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giivmnvzx.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gxqtcjpbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gaxsqfujs.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gunhmhlpc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gneqsqwyl.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gnomyaemu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gxamowjnf.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gamnawrvi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/glcjblawz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdhcqdnly.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ghvdvxhzv.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gnswmpuvy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/glfrprwlh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gulwozeui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gbrqheigy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gxqwskilb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gyzvpeowx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gvssxnsjp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gvtybvjyn.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvbtbkxrd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ggekckcbk.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gryhfbdjr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ghloldneu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/ghqpmtrrj.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/ggwpzvygb.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gazetgqvf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/grzvjgajw.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfurpzs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gndxtftkr.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gmgihzoxs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/guiznmody.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmywfxmaj.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gbsskxzai.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gbmczpcah.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gsdcviezl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwedald.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gajjydvnv.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gorqowylx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/grvqnwxad.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gakfsttvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmirrjtbn.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gwvpztuni.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gohilbdhb.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gdfgtzacz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gvcgwtplu.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gedanieuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gwjsfdvfq.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gdubdpqdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gdeqixljs.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gkokkzhxa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/grbjitxua.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdfkdbtow.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gxcdtahpq.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/goyuppffh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gwczezhwm.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gijdvwvid.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggidmhxuk.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gbnveazgz.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gphmkstsa.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gjepsbnch.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gsysocbvo.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/geyfvsuwk.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gpllgkpfb.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gesoxygzs.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gzoijsjzu.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gahffbtdz.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/ggzxgxnyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjkrlja.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gaxfjrdgk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gttmtjhoi.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gslfshpnf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/genelefoz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbqftxv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/giptqldbk.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gbuiejilp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdlghtaet.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gmlctjqhc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghwqxeqyu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gkvucmkej.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gwuugjxmj.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gbzcdzsqy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gosmnwfip.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gczmdkybu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gvoqefztw.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gudirctjd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/ggpieksxw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gggoyepbw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gjdojrdga.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gwjbyfuoz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/giciqfwgh.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gkzbqjtkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjngqyiu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gaxxfahxv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gjhhueyqu.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gxbellbfr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/ggacpsyxf.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/geffccxkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyjnozb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gocnpvfuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gdzzvbrmo.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/godahfudo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbvkxvpg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gdxntlvvf.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gulxyxqpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghwgkpgoq.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghqgjierx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/givdnnyzd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxxquedxb.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/glsnemhvv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gfwbvwxmx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gblfprltk.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkpycff.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gizxcyuky.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gduuxswoc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/geiyybxql.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gbgdowzwm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gpiltmnju.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gthgwopcv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gewzetpcc.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gxbjxviti.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/glabeoxgg.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gmwousqlf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gnrvalqte.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gogzdveqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gzibglpip.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gdjfqhadp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/glfexnpss.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkcpedxve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gniilwuoo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfvyyhhlt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmsihhaff.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gamukujey.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjqyoikzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gsoairhbn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gvjgrptrm.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gvpcwtebb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gixcnmhiy.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gognflkkp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ggutgrqun.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gtcezcspp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gjklwmlrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbaasxeil.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbxbxrvod.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/guznkddmn.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/goemkxkvo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gxcwglacw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gubwoteps.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gtklwqtgb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwrmdhgsa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gatzodlwj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gaccmvttb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gmnwikcdj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gadhdjkcv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gbnujyvip.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gwydtgvvq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfucycnx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gpnomcawc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwfdypdlb.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gugnepjfb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gwndezulu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghmnnwwar.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfjkwnwra.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gcuytfgef.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gomykcand.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxhcunrue.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gghzhxykk.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gxuciiifr.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gojknhbmy.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gnftkxmlb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gxxfbcwxd.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/giutbbuhq.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/geaotwpog.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gwxnyajpv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gzsjezxto.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/grtmubllr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gcdancpbo.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/geegxuetm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gidmmdmqm.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gppcstbzu.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gcfatxfmx.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/goxkibpzr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gddzsltnv.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gyhmafhky.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gzhtvifyi.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gcasqvxro.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gigdasotd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gtitqlxpx.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gtqukjklw.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gyvjdfmlw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gjigxniot.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geiwmuwhm.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvnqziunn.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gcdwtaovy.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gukstouuy.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gupqgwtdo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gcbmfczeh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gnvyxcmph.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gzbzlqayy.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gdxvkbhjt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmexdottu.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gjdkcreas.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gedrvjxgs.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gggnatqgm.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gcmwrixtb.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gwldvlilj.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gkxlkptxe.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gwxoqovyk.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gvzptlebf.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gwkgqtfyk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gnhpqzqyr.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmlkbsbiv.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gwzusvjie.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gqooltewe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gwzwumgvy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdmodefri.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/ggtgcbixc.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/ggyofhcak.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gveftaurj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gdkqxezti.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gdmybdlxx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gdksqkwut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gkdvutlzb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ghxznreqi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gjspfmgvw.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/ggwgvvpsk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gwrdyyezi.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gcbeurbsk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/glokygxcw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggemkzjxn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gafbngcik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gevigarfw.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnhwpucrv.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghwsttxsw.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/getlzqqcp.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gbdhddmrz.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbwhouwir.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gkrdfqwhs.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/glycgtnkn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gldjvrqck.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gpgghtdqg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gxatuyses.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gnmroqxxe.sHtML


<!-- 参考信息 -->