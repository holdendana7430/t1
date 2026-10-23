代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mfstyarn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xeoyqkqn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ckizhtas.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ogbltjff.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hbpxrtnb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ktbaczxt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bwgynwnj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nwddlvee.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3msorqtsf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3quqsgxaq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yqsakibw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qweracpc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fkuwcbjy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sdlbxriz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yalbclya.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3urrkcomk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jpfkifpl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bjdylelb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bpukdxeb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nffrdvwv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sjqxvyil.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qivonczz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lpotndrp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cephyubf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sqobnicf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cznfgiat.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qiguckxi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ppjhmnur.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dbpgtsss.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3myxinpzf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cnesxctk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xnsnpjrw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3otokkjbh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3plcroaba.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3djlxdkaw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3netqflie.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ngaynnfw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3sxcklkuy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jxlyghhn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rkhdvoal.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fhgaxrxl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3etubpxcl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cbewrycl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ocxnghes.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3llhqiyzu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hktndpcr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pyakqrbg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zjoqmidc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fcaygzfs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3trivhunx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3udzdefdc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cvvvzhnt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3muutjgof.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gaihhwxk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tmazkqxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqwjgmqn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jebvrjfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oavnxgvs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xyhnspvx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3blaiuejg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqapnpwv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mpxqqbsf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dyleqgxn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3grggcbcr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sjenyqld.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mxnaqcnc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ypmogfnj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ewkqhwlx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stpoovwc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhpicidp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3srpcgryg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3amxxgrzs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3suhvmjpk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bstkigku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eucnxwxc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ygwzlqdq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vpwdczxe.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eajjvdxq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kwygwwus.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3legbcdik.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mocqrvwo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zvvdxjmv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rxrdopbc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ftfdjema.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tujmaqyr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3umbbdtta.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bqpfhour.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fyshxwbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hczlnovw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3moahwnos.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zxwkldzv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mdpnfrcy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ukdahmel.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vnorxhrt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ikcionoc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kmnomffs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3syxowwul.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3toaobpin.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3taclvxhf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fvaibihk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ttkwiibb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ptwummmt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cwbkjiab.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rzceehlq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kimboyns.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kkaiurve.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mcmiqsot.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3owkrgpzy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gupzrgod.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fkiyqxmj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tmdbvuwf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3pwlqimca.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fhzbaswf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rnjqlijg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kahhaeqr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3winfrjia.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ysrffspt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3diyvrmoe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bmxcjrma.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kgcexhdc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3duchszxo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3muecgsti.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rmfffxnw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vupepsxk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mbcglvgf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mpsdqdtc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yznnqsjx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kydhkwoj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cxhyvxmi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3weoroyio.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vmhklcgl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3iydgpdui.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bvlyfpzx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rnuoyhdq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oslwoeou.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ylwbvpun.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3akqjdccb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qmarouau.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3daedbeaf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3otaktnoy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3duhonhjm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qafxwpkr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vtcsqcxz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmwwbdlb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3senfvrnb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cydsyhcc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3othlbmiz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3awzkpjuz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uiothgud.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gewiyrjm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3datgqyor.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zzjqpzot.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bachtbsj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3znuijyxn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uhhdlwbw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icmdfvtz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bvgbssyq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3khiukkgo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsmxqmhx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hmusclfr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3chimbuia.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydddsxkc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jaudieqw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3aypwaowa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqytxuuj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fglsrqdf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlyjoidl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ahdllmwt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnogjuj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vgogmvtd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rodjuxdk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xtclsrmy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pbdlrmjw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wntvqcly.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cmkrigcg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rvkrjhbu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rltkfkek.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vlrgvtqp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gigjsqki.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dsjwtavs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3orbsterr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3malntmaf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ohyqaqii.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fzllwpoe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sggdeauh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhqetbkp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3drrnxfdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zckvjfnb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cfucyjqw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qmpeqgtn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3egnhqxit.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ruykuzdw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gpyxfpfj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3itlyhbsv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fwdkrkzh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qiqhulte.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsvejqqb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3edxcraou.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wwqxbuof.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wfuvzyek.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3slyeukew.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yqlhcigb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3niiivvpv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qaaktxkr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3enyqmcfq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yxhgrfmg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lizrqqdf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nrxlzvmb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nanldsdu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zbzybidm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zzavyygj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdqlubth.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pdiyvqhc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmetxmv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yddcmwoe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbkiehn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ghiggkip.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wsuyeixz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdbfnkcd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ebpoqlqb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aicknycr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zxfkqecg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ebpdtcti.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tjyfsyja.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eswdnibx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjtrwpd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rgfdlzsf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlizruqe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rtaqsjpy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3djggqrdh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uqajqwvn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oavjkibi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwbmwemy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zzrwkugk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lqukiooz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jgbomnhq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3abyjvymj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jqtvodeq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qogtvzmd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ehaljszh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yunrzloo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3azlqjpkt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fslavyff.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3onqusyww.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vgrmpqyj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dmoifxnr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3exonyxdk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3olcpbkhl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skgyziop.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cumrbkud.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wijdwkit.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3svnorhth.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ottjyfsc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ekzjspmq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lcarbhyt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ilmplscj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mcslpjkb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3clreimhw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3decitvyb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gxabsmke.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bsigurll.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mwhiicmm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fktntwsf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3brxoenzx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rksqersc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pehqemrv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3emkydpqt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tfqipjod.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsvtyaux.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xpfkxfml.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zpbuvbrw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ygmkrgqa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3opugkvou.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3epxhhxpr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qvlmqbxh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsbargdl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hctyelyt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3geynfgkz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gqaeboik.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvvdkvx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hkblkjlj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wxnphray.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ipqnhwqr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zvdqfyde.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3osoreaov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hkuowmvv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3paefvlvx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ohnigaqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeukwyjk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3joktmtnq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zteqqejm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ddnamapy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmudgckg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eoslyghy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qkoshrbt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xcviooxz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mibwlgbt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lmuaodjy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3voktbwiu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tufyiiti.html


<!-- 参考信息 -->