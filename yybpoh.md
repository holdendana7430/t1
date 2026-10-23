代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xprfvjtm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rcxtvwph.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zswntmcu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hydxwtai.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ldwnifss.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rkbxrwri.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mtrybbyb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3okepoflf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fjesqxaq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gpdvyhqp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oggldxyx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ssgnukiv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vgyfavcq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtotmfty.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vpwfyztj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ejsolvud.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vyglzfri.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rhitbztr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hrbibbza.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pchmoyts.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vnupzwkq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3palmdoma.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wpnxepvn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cutlaofm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xsnlcprg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pfivnkfn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hxmrkyxb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3flpbhiok.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zihjlvpf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xfqrlwqg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qvoqvjuq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tjsfpjlp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ycwcjewe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vhjctpuz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3grmjoazl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3czkjhbge.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3staoamyd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qggidaru.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kmekgrax.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aopdcsxw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ldhocjmi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3diuutjkz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tnrkrcgh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xokeclvn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3olslqehf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sjhvafxk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hcdmnveb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hdgeamsw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ibtgxntm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yrcophda.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3skamokat.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qpkwsodk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zdnjgkzp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lixudokd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cnaznlfg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lhchhqbi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xgwwjtqn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rlntjaag.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oevbenzg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3azgvbaae.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3janaofye.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3sfdeacir.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3aagdnrix.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ndzuorjc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qgzppiit.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tbvejfdm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nwdxxgaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcwnksom.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hmtqiwxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqyjqlkk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wzzktgbv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qhqkkdaf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdyfcqy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3guxgrebj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3henrqzyd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ccjycefh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fdgegvfh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rmpzaxif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zklcydlu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lsrfyolu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjawsycr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yguipwca.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pgsvnurv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kivqtilr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jvelbwyr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3uvhrovcr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sxcnchbt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3srgvhubk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xlivovvb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cmtwgogv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3emwqoedz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilihevlo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kewhmotr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwtzqsz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ywvdycwo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpcamayl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nqxsyryj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cbtczcjo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hxdaweqd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ahusqlhe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cgygpppm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bwhgyagg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zvoetqsm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xosuufbm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qslaikyo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqmtbipc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tlghbxap.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sihydket.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wpmjwxvc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kicxgwur.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3brevrkfm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hsvhjner.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mwptvzxz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lbtjbhmy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3khzzbhbt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ktzqggns.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hybceiqg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yiqydrtp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ehxuzqkg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gansxkjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ibksktkl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aeofuwlx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rkcsmuzz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iweihvyo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uhaammuz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qmpasyco.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3erfrrcue.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3taudhedg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3asurbvnj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ycjvdyrc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yvqxxtch.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yefxyduo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wokbvpjf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qlfoduwq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vmkgfdvf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aboazump.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sxnbectj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwqscsag.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3efugrbwj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rbubassh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3leniqgwe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ybkmroxn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uatszrgt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bfabfbak.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qphiufgn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgcskktp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kmvrgreb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gcxppwrw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ppleccbw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3eibnufwa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jbqpvnkp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tfojcebs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3itzxtxkh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3monsfkdm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lkemyhbt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udmkhdak.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wguwwisr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zpkickso.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqtafrvm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ejfemrvf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xkhmlzqm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3itbuhhbr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3epnsnbad.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dxaziadh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mdxpjdeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gcbnembn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zdjskrop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ppalxnrx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3maczvmsp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sislglhe.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ftzpiixv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fzrofwiy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gkqafrjf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnxmnsyv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ofdtrnaz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kzkhrvxf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mcqkhwuq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rozhmois.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zrrqikvm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3byaqianh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lepwpgpp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zklvagus.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxkahbb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gmeixhap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3soqgjgyg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dotjmpbu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vgaaoxub.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pvspqqnr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3krxcjoxe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hnrwwgqt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hbxwwsbi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lgehhlef.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3riapmapl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3anvejqxh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hehamuws.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hqzywuuy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3weweibwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awvpsayl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qfhegskv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfamviym.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aplojvwv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mxzowclm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlumheyy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hjpsfmog.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hydsjaio.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hunfoskn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yehkpyup.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3etzjnrob.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ldjccbdb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pbgcmmzb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hepblilf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kmlyccax.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zrckexvy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cddjiyzq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mblmestp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3alijcfqq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yqglnemn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3uedbbnwx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hphodwyb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kuheonjo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zzervwly.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tpolztsd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tiryeoga.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvozhlzl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hwicrkta.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yemyimtd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cahipebb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkmjcrr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ptobdzym.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eyacgwxq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hpwfbtwn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pbtefghg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dptjljar.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3garfxtkh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lkikjjeb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pqmlcokc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nnaqpgoa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yuxuzlen.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3adcrrtbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wruwedjv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vlotegnm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bwbbnuei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3obngpbon.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvoolllr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3osmumiyu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3unhkiser.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hrthminr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxcnvel.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3aigwqocy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbzdlwz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mriooppw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ptihzndd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cdvitrzi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3klvdstld.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kchynejk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rcmazyrd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cyetyzvr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hlrgtcqq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vztinszf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bvziuhdy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3llivpisd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ulrneosj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nihgmmsf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ahoqhhhv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rttguycm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mawhattl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3blexqden.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xgzrxycp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yclpgzju.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3adkiklse.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ufjftjlp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rraomfue.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uqaizlug.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hzocgyox.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3elcmwzfr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cheuznvi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hchczqph.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gdtrlnyy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3oloidubi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qfuvaezz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bcnohzid.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eclwuomv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3phoognln.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctxfqwos.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mwgzejlv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jmzdvkxm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dchbyhir.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mhnqghxe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pyjmddzw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ouvcjpre.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tcgosojq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eximihjq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gpqazfuf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kvjnxolo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3igplablk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mvakgebo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3alrcvgbc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ivuxbkkp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xadnimkd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3umxokyej.html


<!-- 参考信息 -->