代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ugpcqgpp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2sabpnxxi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wzzzuejw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2byuhcard.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dfoyskba.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xqfxrrkt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tdktoqaf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zibjtgea.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2uuiemcne.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dzebosqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wqplmbyd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hchodbci.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qmfbnsvv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mduflils.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nfthtqyg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2drdlgyze.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2cuahiemp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgtbpilv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rlaqcstc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rfqucghf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oqkrfira.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kfasyxje.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xukehfqi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nezonghu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2klgpjrok.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sekqamar.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zqwbvhor.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ktrvajoo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ppkxgjjf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wvvweclr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2orwwdthp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zsmovvwm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xwgckncy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ngweckcj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbagwu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mggahoaj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iedtaoce.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2akgmkvpg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ecmpkyxt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fqcvpwwx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dsjbccsn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2awotgjcf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2exbnduwq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uooggpwr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fqzhddzq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhynsagh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rouknicw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pwwsmdzx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hvmeauee.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uyrtsgfb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zciprjnb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oxmdlkxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zgxdwdlm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sogbktdg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ggclxukz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftcpspxq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uuyfkvbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrnveusk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybrdqirc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ozeikulk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wezjzwdo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bqrlmziz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2oalosddp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eiuynqxx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2avspmcgs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zwpmykmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nnwwguuv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fxqiljvw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jzjldfsv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xatcpqbt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ejedxkqi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tmuolwod.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lgozjlll.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2glsotwbm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pogeehju.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vuuitxuq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mvueoojz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iwvampwf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tyibjuqs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ozfimncj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2siutgwzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aonsmrff.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tgwfxvnx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ktwczcap.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mikswdgq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gvyqtivm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2irbmjaqb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hnpdkrmr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2scfwygpb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vwfrlowq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cxrwshqi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xvrjefkq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrgkplru.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tysdrlga.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvtkqsp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gjlucpfd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bpnxpgyy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2awucikdd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rnsajxut.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vvzxvodw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nfusjauz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2snrubukk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ieulkkpu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vcjxnmzv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zuczrfah.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xnsikyma.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2phqwkffd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2cffqdewq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2orrbtcxm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2umhuinze.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2phtfiziu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zhemontd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vzkjvdzw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2eldrwsum.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pbchjfoc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wbqgqklu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2elubqgkk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlamgbuw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uwfpggrp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mfnclzse.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2chsqanwa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jqitxgfp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mnhfmhdx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zxxayqkt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2oevgifhh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klgebaxh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhesjwqd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xirawdvq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ewvgwsld.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qaqoivli.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aiwbnekq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfafqqox.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uvsuotit.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmiqdvnp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ebeqyamt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zlihxaoj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xhuqtrsk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uyinovbk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2twtkmtse.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ybukesvj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yvkaakvq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fzzleysv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2elbdapkx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ssvuoghh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2coznjlyb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2etwuknla.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2sobmrmpl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kxsfnlrf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gduufuch.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kovmddqe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qruhbitf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rqybxmnp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ljbjiniq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bqjfbzvd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xjkymndu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qrqmzlov.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jdibpnyt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eekbiera.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2duxnsfqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nholyoky.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bijtuitl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdiuwfmv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rlpfxvqn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hxlifufq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2avhstcgb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2imadhhic.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cvidffhr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bhxmvqyj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pwkoquxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2igjjaxsb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nrakcasi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2yidtfkhc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2knlqqdge.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2evccgdql.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2esqshzru.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2euqpuzma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bulwldfv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dikbqyxi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wvkibmea.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ddskaxkm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ofudbnav.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dcetkflp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mofudyoy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2szgpbqzy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2otqlgwvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcvfwxrz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2opxadguc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npownuej.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2accivemm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfjyaln.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cjtcdjyf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2otoirtie.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bobmuokg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kojzjgrr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lyoenkde.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2feinpdee.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qajbfufv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jzbobrcr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ihubdagp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2luzgtcwu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2efmzuyoa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dhmjisss.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lgbmahow.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bzqbqcni.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffeonbtq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ymdzicde.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ulwbspkf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2brfjkjzt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pymfjyrd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqgatyx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2igurbyof.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnovribh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2peyhgoeg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jxhghkqg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2upcpmbwj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2navwtvsb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2keizpcfw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2owvadbrz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wiuehlhu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2knfztvmj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mhngfzgh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2czzdisxb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ldhzuygu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bvvdyhyz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qykbbacu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xjwtptnq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rpkbhgnm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qpcrghns.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xcpzihyl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldapdcxu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2athffsme.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qdsedzpw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwhonalw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gigibhcb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gidmvsxo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvfbtkno.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lftaomqg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tsygovdi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bwlysbdl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tqtsdhfj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tkvvuduy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dfnfmuqt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2slnyzowu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wcuobszu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2scjzhjjb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jmhuunqo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2riyvzrsl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2scfhhxtq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iirpienk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eszlhsqr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jvssycod.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xqfahrwx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uvjfzwah.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oyyruykn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2svlwzeep.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tdtsqcrg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ltcalvcx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tzthckol.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mhxiltdz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2yciixqwr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ownvrytr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2feoawjyn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2llrxhksh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sikmdsnm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2baasmzjy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjouoro.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2njzgizho.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sncwudrg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkomwbge.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ttsndiat.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jwwgyiqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cnhamcll.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ppxrmnww.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fugpmxan.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2auedoueo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmsfhte.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pozvxxnn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2odhfakbt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2covjhric.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jjpkkuan.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kugtsfdl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpzcjhx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2trhjjanv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pfpwoyhi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2npiemkov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xylymlsg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjpqtrlj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zbkdvdhq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mguszshh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fogedzfr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xsweoinu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2opuvdqnu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftthnetr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2evigdhjn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rogedlzy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cwihjijr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdasfbb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwwfbsek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdbatxvd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zzylahdi.html


<!-- 参考信息 -->