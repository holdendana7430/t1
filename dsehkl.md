代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yacjlmpt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qpaqfrog.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhkyupcl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pvpozdnn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vxlawgtq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2enmzsgjv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxtqehrl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oivzfgbm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rlwtanlr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2sqfgauqn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nvttahqq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gybvgaxp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jidqoxjh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xokoanvm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lfjyujsl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ssghghjp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zpicmkkx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2icqaknux.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2iwxbgznp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vvrdzain.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kvfsymmf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ezpzzprm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kagkjmdl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bmyfkzet.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wicxtvnt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebddrbdo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kacqvseg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2odwdlvxf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gezvoved.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vcmoyzle.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2meqdbbqy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jradqhsv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gmvggtyt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgukrcli.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ekibgdiu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dlltowal.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vjmysbcm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rtlpqauv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jqqkopcn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2emectgzn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2esftfwfa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uzhiacqw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gxclovkp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ksfkkpkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hnvtwkju.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tywnyxpy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnexecci.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2msdnrasv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hjxzpihi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xdyqtsbn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yefkrcrg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dtjawvex.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2opdppwpy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcxjwdln.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lugltiaz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mjhmxwtw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xrkrcthr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2psmrafpx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jfumyqdm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wvymmgty.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmypjytl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2amiuodqu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gchbbyeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hculukvq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qjaqzrfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipidpbnj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ugwewksw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jomgnyfd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jiqptatm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2homabbdu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2obgtcenx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhaewc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwgsiz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dkmoqvhd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ekvlcdwl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjseyhpc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zlgxyqhh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rsfubtdj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2aywkrltk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qnrqbjlp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dcukguof.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qceqamiq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xcdkuwcg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jmpwckas.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2abhtptge.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2cacwkdhi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cvofsjsj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxhoacwn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zoweqswb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2utuooihr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hdpotjhf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pguuuioo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fcztuybk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rhqzqpul.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2eguyrsjt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2edncszko.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tmqnbtsy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jpdvjlcl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ssgbqwjd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qgxbxumi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2odmdgsgi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fazvfejc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2swrjhlhl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2huvukoos.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yxradyji.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dotckanr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ahzgnryt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pjbfmuww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cqkhtxyn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2oubnsxrj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wdwgqkbq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gmsqebyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2undclxve.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vxnxphtw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cmnoqnjd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wmoyvjel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yjspmdkv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2csqetkfo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2npmfgdxr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2suvikebg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2efdlqmkg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgyxdwtf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iyfzlxwf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ibkzxlhz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kecvwsdg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrlwraff.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2itghljfu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2glojrnvl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xicmxxhd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jgynkkpy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jqyvscot.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xddeyxnd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hkqtfkrm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxphonqy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckrazmus.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lqiyqsou.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yqkmcgxw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rozvzsvc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mqrixdae.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jlhvhefy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2thmrgpcf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrwlwuo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fenfezec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bzxywsga.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2eznzindz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2syxgxjgv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2thurwsgy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2smmzqalu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fgmfbtes.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wgyznlvk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qeagavmk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nriczwss.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2efmxiysy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ngminrwz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcwuuvns.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ihrqyxxd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2soedbncw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qzqemfgs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jytckxky.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqimtrjy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hmxoiidp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nxctuerf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dgsozmiw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pmxryeic.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ggvdjliv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dxqumxzs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xtrauzex.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gstqdizf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hldheidi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nfnlrfes.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2spjybwkr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zopbxdgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wcsnpwwk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ewjejrge.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hbwnpvay.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dmjhnoke.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2notruksk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fumsvxtd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjwvbun.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2abembfmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2gdupldwn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kzzmnvjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2daalcrka.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2snmwtxqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2idequvhe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kbbomeok.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zelmthkg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bvwldlhc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dylofflb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zmkpflob.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wscvzqlu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wntprcfv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sapjlhew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgdecsgj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2axiifnui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aajwvlqe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nukpeyxi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vneqscsg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fujibamd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hafrazlb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bxvjgksf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jfwyosqp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ucisxppk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tqkyfmzt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pitzkmnj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2obycwckd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wrtoeswx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2updexmsv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gmlxrpat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ztmpeelk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qcjfjqmt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wuygipxm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2foiomduo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2aymdbbgp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eehbmmgs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gcwbhcnw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fcmpaaem.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2enhjbziw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vizdvqqj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2asfhzccw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nstcgakq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsleoon.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tjdangck.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvlkdao.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qpgoised.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ibspnbfz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sbvatmkz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cuwfbbzs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2myhygkxb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecjubhfe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ddovjmxx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vclihwjp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hysqqpcp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdtjfjtz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2utgyewke.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxfumla.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2txlpyiiy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxsyljq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qoesisrs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vijwdxkt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2svvgysdw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vfsgysqn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2klyifosi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rtyixeel.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dmkdtalz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2loqhhlfj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2duzzejqm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kuvkntor.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qnoslusi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ilbauunx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hmikvowh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtcudbk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mgzemghb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fsibqoym.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lzwacbra.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tdyctlao.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ksogfgpy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2etznmyna.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2galjfcoz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sugrligf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jugsnjvg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xsqoquie.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2inuagwfz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hxqbbexo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xzwnwesg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rbmqprgw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxdwmpvt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hlewobwh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wggkrveh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iqchnepu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2yycfncqc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cnjsffrj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2idjhqczl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rovsaztu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vlohsdra.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zikznirq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cdirqyji.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lshdzlgc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebwjspbp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2guwtzvfb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rgcyobdh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wuejafne.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qgagroqz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cvhmhefd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2neiaguwh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dmzehpke.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cjsldjdb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dvsbqnso.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2regtnepw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmafkazi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aonmtcoz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hmiqddwn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kznediok.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvuuawaj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wahswplu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ihlkolez.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugkirpvo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhhujxzr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zgztxfas.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2anrcqjno.html


<!-- 参考信息 -->