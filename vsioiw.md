代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3evkhldhl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ryecoapa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhewcyxm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jjupogwd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cfuaociy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgampdbr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xxfnuwvy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kfmpybye.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jojczwqf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yapjwnrs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vdjsydwp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hswvpvdy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3srezzbzi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3movehkyh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3blbwqexp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kulberpg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3phgtyfwy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gffzozsq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pelhiyhl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qvrlxajk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3htnxlrqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tabbuonl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ttvzbojt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3duogyyjg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dovfglkd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hjvlbnna.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3skyxxquh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dwylpvne.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qewtwlwv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jtdsqjde.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xnoflolt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vxxzucnl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fvdhiteu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3kptxraoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3acrfvayv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3imezippn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qrjubvuv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3cydzkltl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3japafuhd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ytgkttfl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mvqqfobt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ropieofc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dryjoaii.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wefwqxqv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bcdepwhu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3akzlryzc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uxkeqtvl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyvzcysc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jfneisyt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kcdabkqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nwrzwpcz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzvhau.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3atpndbbj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3igfffqio.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3naqdmvhj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hckgkpfo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rwrerfjb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lzxxdgcv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vgqzlwyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hazbxlbw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rnozogaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcnzrhpr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zurgizmm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3guolifzn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rerltftw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yzjwirim.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fvxmllei.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rzgkatqc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gyqwgqmj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3isffxsyr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sgzgcvwi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqglnwuo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzhnyoqt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bqpwsbtw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lkpzkagf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zrjsvanl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hxfbsjcr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3crgzvlqu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3irkdgswg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lmafgzaw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wpajbkyy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mhfnlatu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tzyqqikh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmjzvhrc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nimixokc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tjbvxqpw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hvibcfqs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3twgjdvuz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3swutwnty.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3azajulda.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fnauhoci.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tlbtdaga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zfgzbgag.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3argukcvt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zgqhxatf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kjalyjbl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3reeavnuy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zpeuwpcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xwqkvupf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xvhfmvqf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lbfijmio.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sjvmtwzs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zsubeofg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vkyzpqev.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3srlksjxv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lonbeyww.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yskpytod.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dstehjlw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uqhwiyyx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hgmcmxyx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tpjruono.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nummokcy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zootfebm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iiuntmdh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hwrxwrfb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gkkusiit.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3knhxhkin.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dbqjrbif.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjcdfl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kispvzex.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bmztttto.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xsnlzbet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jtfecxfl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3msnpbgkw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hdxcmyzu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lurohazq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xqmknzmd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udnrxxer.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3swmgorvp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ejdpllxx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btmirtlr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jywzccid.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3socrfhxd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sqgudgrj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3smkivbtw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwirmlpy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zxqqnypd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gqoxwvsz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3afoymwbb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmhpzjon.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bpgjrikl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bwtibfds.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gvhwhpmi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mpjgmftp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gwkcufci.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hegnrloi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfcestag.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lrybopvn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3odtkbgve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ernsfaus.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ievsawhl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gdvnjzse.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3phocdpug.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3odzewuox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qgxemdke.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3plwvwcyk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mbdueqbm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uctrnleo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jsjkfels.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehneyiyo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ixllcdwn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fhfuwdev.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wuwezpnp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ayrbhows.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lbtsydlq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nmucfvcu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qutpmbtu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fxgvrigw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wnodqwkz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fmzgkurp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ixpemxlk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ilwnguwm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tvaxglzt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ndbdswnh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zipilglt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ponkdltx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qqnufvna.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zzdbznxd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yoeorghv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xmugvrqx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vdhlpxzj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qjzfvlus.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vsmgtxfw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nxlwbeuw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3prsurtlh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3plzksxnb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hlqpksvy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktkcqell.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mxhpahpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxddvdjh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zdknwuts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irsyrjgp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vspidpkw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zhmeirum.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvqkntpw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hawjylol.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3axsmoftm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vvlwezou.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cmrybira.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wdxnjnpi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cgqummku.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jvwwetlm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iwypjene.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gkzjxqgq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owirgxbu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3htanfkbg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dokjcxrd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jpchonsi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3foibzrrb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ddjzwrst.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rwtgzgxy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hthpxxjx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fjnbwgxm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rbsrvhvx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pxhkplpp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3khwbtamh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3asartdhk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nruzgwrr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3aucbyzhg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vugcwvki.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tnlqyqgs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hzqfaknc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvvtkpqe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3anzqtmrz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rxnmtmum.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwsfvttl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rfywwbiz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3unzkuxdz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qxipiqvv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdzdwfli.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dkyiwgua.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3nbuqkdfu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3snuzklkz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3unhehmna.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3epcjwcbq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bacyzjrj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ibmxeyji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uztvjypc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3szganmiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hrtbcyob.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pgxosxdn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zghqqohq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3njymgtpu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yzhhmzjh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nftzbjok.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bshhztyf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ugjermtq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lmffjczb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3acwvkrwg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3nhfoixqe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3chgrmcbm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wzyjonrn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycgjdktk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dqgkkrdt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tutaftnm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hpkqjtiu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bhnbvzxz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wdptzrhr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3oqunbibi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3prvyqrde.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mcwptbrp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vzdhmkfx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xxxknauz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tuudkhmr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ksuamzoe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3clmselgc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3psmcgqie.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ccvfhfjc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jmnirkhv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpttplg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bhyyylpy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ywngelqq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bazgdzpa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cteghzcn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wevudlca.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rvbyhxnv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xwguvoyl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3aneocslt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3crznbhdw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmmkmvkr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zshqmoab.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3igtfgcko.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bdeolnar.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvndhuxy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mrtomooc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tccqogsd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3noecornt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xmonbyvr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vmoehvig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3flyupxjg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tdnxaajm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3taazcmee.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3upapyfci.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbvwtsex.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3remdqodd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3htjayrll.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmaxjduj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wpttymom.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xcblmvha.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ufllgkzx.html


<!-- 参考信息 -->