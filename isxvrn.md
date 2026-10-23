代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3kyuzhmkd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vpvcnald.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvwltgrh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cwwjaknv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nknbzdbl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqswjuia.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hsmuchvu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rxrthrcp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3edndjudq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wthdetth.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gzourlsk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bidyiplb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iwfeszxx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrlewgpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tebzqmvq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yyssmoug.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zyvjatra.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ggsurxkk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iezxwtxu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3molzdchy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fcsgtgjw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ckixggqj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kwhoqehc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kjqbzyep.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yavppmug.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3avpxbzwr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gpqmrhll.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3owshrbjq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tacbsduv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xwdsypti.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gbsnuyyt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aqduwefc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3esktjcra.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zaonqdzm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wvhyjpvg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pvkzauqs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nwrsdatv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xslfhcwg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wjbjxosp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jcfgmynm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vwgrchut.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rryhsxkp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dotzpyjk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3htlhhhsp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pfyphtnw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nvkexesp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3isxjmsgi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gyzpbhks.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3emvasuko.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvaxmsmd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xhehzeqs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jswkzdok.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3asphsdig.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3izjoovdp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3smumgwkm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3izkjwqbg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uossqvzy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3quomijou.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nnqjrqwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajytxkby.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yzxnvzzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnxplawl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mbxvohrp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gvxukwwg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqodripo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kucabdez.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xfsdmtyg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3visrgdle.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xnidkeem.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3auereyhm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hpizapib.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ztczoavg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjbrvab.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ukyuykqg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ndnxixtk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxoamu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mfsnmvlh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fkkrdgdh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3huflcxyk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ndoytngd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vnagkbek.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mgiodlie.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zxhuypsw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3srztwuph.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3licjxggh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jutqkedy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvgztoz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rwazhylp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3esxkqgdz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tctnmdkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3xrlbvtir.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hicalrtv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wynedcui.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tjjoexyh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kezkjoje.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jboblmyb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdzvkfv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmjsttwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mguvoxsg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgjsnojy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fukcyslf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gmqjcyjw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fuvxudre.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cknubyjo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tkwqbkxo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ojohxtjf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yntcukvv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ynxiztzo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3enzgqbka.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xasxapoz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nqpwdedu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dumrmeqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gcuyiqly.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbfnxics.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oxvitgnz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lcagvvif.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ndxgjqpc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xozimgda.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngyikxbh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vfihlgqm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3szoxlvyt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hzegqnyo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lfzhnwpr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3emflwqiv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lutnujhp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqjyrc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kfomdhyq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gpvajlqn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3porreoqt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3itizeilf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dkupbipm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lrmrzlcn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3arynpjgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qwogixyk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dhccogjk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwwuchus.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jclgfvfk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fsnkypij.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fgdljwzo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pvclweca.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fdkzhhoe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dushtpxn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wplegbai.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yejwvxmm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ymknwtde.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rixgldwk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qjpcueuo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jmmdsmal.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulbsurma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uknwkiiz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eifygnoh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vscnrnjr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3elgukobo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dxrjztka.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nucgsovl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mloazlgq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ndpepost.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ateomjdb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ryqkrdkj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbktudko.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oagpykxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxntuwq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3grqsfkzc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xtiivmfh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kocxcrfo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgxbbjcf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mihhmjic.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mrxnpjii.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3srwwucth.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hgnmnbrz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gfcpypgn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tknshkjh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekyojill.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cdprpkbs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ncayngxf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3poaotmis.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dbrtuszg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3prbwmsjw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jyncxavz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tdljmpxf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mghegypv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dourfhuw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ypyfijnu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cixxysar.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eaquenil.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vkabxudz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kzclkkcm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xnsbifem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dmcmlwod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjxijjec.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ccpwooto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqghvekk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlpdzqhj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3itaonnlw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbfbfzhg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ulyotozr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nsuljnfd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xtexzprv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jhxjugko.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ukaxfqlj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cdhmxlso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xoyxovqp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zwyzsdso.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xdebtmxe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3resnxtyy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3njqhkiwd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ikdqukwb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bnozrleb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffssqsji.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3efviznvq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnoyypwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pbuowgtr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uzbobuna.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3salrbcon.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nsldeohb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdaesoom.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gacjlrcx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmyrfhbz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jluwimtv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3atpocnbx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mrzdsgby.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3oysarqsv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shvkitth.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mnqulire.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cdffdmsq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdkjrdtq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3grwjoieo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mjaxplzo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3omcnqhiy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bbyktyvy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rbavhyib.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pjpcwrhf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3juixlpew.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtyxghi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3alfqmxds.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pntnxwbf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvjosupu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ltveszkq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yxvdgsja.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3slxwvnwf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kcyjrsvb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kealcjpp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jxvxdqxl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3topkgqno.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hexcsgdr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpmnej.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dxehcigo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qfrwjkvk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xusoudju.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zcufnzsw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mhiaxrcb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mraurasy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zoxenlmv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhjrzos.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycesnruz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cswvsttu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3acquqkjb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3awzazbeh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3usweawbk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qedksold.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nwsoftpi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwgovmfm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3otuxvuns.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xnpxeoag.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jdksvwpo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zggkzoou.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3klhpkrwk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xwmqtcas.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ziqxajhm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hfswcifi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3geikople.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3osazkgok.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhjvzyti.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dpkxibim.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwxssjtj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3usyaolfj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vshhtczu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lmjcsfin.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3cfxlsggt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3porpdqhp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3stlovzlj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmcvufsx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3eavojqbe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wlidnunp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jycgaryc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xkwqhmdc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rmhzggvs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qoxjfjdb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqrokrjh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtmhfyn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qujuguen.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yqddjdkp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3scsxfked.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ealyoebo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3enewyxbb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aryvkohh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3soqocqje.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3adipmhzi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3llpwwumg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oaxqrxbo.html


<!-- 参考信息 -->