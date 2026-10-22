代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tzphswxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sjorjobl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cmiklgpz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cinwidxe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2itailstb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gmoytjad.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dxaubukw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2reoejfix.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2liathbqu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kpoyxstu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wudjsbuu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pwqexqpg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hpnopyhl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dgbtdesn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2courmgkb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wcmgwyvm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2parujguc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2decgsacp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pizmtoeh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sgjbnhpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqofku.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulipmhmg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2srwpjmbx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kzchutvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qcxshbnk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ayjuwwfq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mhhcuzmk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zerwgeaf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2prvwzzjv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwlbqqat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pkmqgtux.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hrsdsqyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rhtwuube.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fbufzbdh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ubyquzav.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ozajiale.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wptfcnfn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2iivqaquw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yorkplft.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mtppsvet.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2afobkmmo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2upxzlodo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rseaahik.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2sayvuwjr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cjdezgdy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2brnugpjz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yyyuwjcw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ugdhelxp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iqrrmcmu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2njsfhlwe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwkozdtm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sbeyzpfj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uihkpvvw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2stuvmvst.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2egsrmodl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqvecoio.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fqmwzrfv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mpmnrhyp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xnofkarm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tdjejygx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ekscjyom.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2beefwqgf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2txywzcxb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vvajeemh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qmzptbdn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zylwdnat.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fhzpmmab.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cqvtmpbj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nhracyqj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nzleflhh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tsvafzbs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2avmynglu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yggbpegk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uupqamrd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rdbxkcsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrcuydil.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xxmrzwal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxxncseg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbwqqnog.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wjulutyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmgmfqfy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2khscnuxr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wsomainj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lysxvjnk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ehkhbxhl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rfyfxaud.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hkomxuxd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sapstdnf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdurnsg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjnwacuf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2okblmsam.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cifnrdjd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qtotcrrd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2amgutriq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqfbuh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gtzbgzjn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2crifobvw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ndtaahpa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eccdjfup.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gnrkrlde.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ddikzrib.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2plxklpuu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2anehmxoh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfyvjukc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vmisljeq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rmdpvqnx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2owhgtobv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jtxalppf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hgajckrh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xvwmxjqz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sggaevqw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ytmilvgy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hakknxvy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lhrhqpft.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lcnuchsb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zepiqldi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jjitwwyw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wmuqlnkj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fgbhujpk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xxgpqghk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gfzzeres.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qqtwrmcq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wwesctey.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xsohavgf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2knlucrqp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bbwazxll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oleieouf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gbkqkymi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xarcqbub.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2riwhwhzs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ahhbkhni.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zjfvqxff.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2yzfidnig.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gtyvnvbx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pvizhtgt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dpbjbnbu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lxbotiuo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqvkkpoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mzkydkcy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kpoqiikf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mrnbeagt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uiziwoim.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lxjuizyl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owfdualv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vosnjqjr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chhtbkts.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbmiecmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2magorhou.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cpkwxemi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tdjoowyy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wytdxwfo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2plahznhd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2denjoent.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wiunzkjk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lzklabhr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2swngojux.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iwqecczw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lxuxfivr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gnioheir.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iikkjxze.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnhbkqun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fyaulsxi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2csaxqpsm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qoqrckrs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhfhyomz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yjgqgdgg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vhpncvhw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2leydzljk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2keucaszk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kiicbiha.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hzfofkyj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqunwfox.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nuavqrey.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pamvhxva.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mxxoustu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vtcxzkfq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2komifhou.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyuajpt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rluwurgg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzusilx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fpvzhpnj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2syicrbbu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rrfrdabm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mcrhzzav.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rihssnrh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jniyxvtf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uzqblbbh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zcocubaa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sorrxhwq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iqnbiyjr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2izddavns.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2leykmakk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vqqrehod.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vcwcrgxi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2eexuevul.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eujypedk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ukmitbvh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wiojxzai.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2athjdwsf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bdazletd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kuwrcpbs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cueifdwl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vfxpcokl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ksspssdq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iusggsip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsbotscf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ydymkusb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tefryosh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tuzmfaju.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nhuzbiik.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dutquxto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sebcpjav.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lityuzxn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2evpnlcsx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2aaniwmop.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qblymxgl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2doixbhox.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2azbygnfn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2thqbgsgl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yvxlnose.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hdxugzjd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vpjxibnf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cslvlimn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2baszmnbm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngdtbojw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2morkpitb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pfucxfat.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dxmgkwgy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eushmkax.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lebfxpmh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pdketnyz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ejbqisfz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oiufhzrp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iarggnem.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2icqckrqk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtlyas.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2eefqdvpr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vvytdjmx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oplbjfmk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kvwyapyd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qpmeafrw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2frqxmjdz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wpnytpzo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zxwsjwjm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dpsofmrf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tbhwrhji.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2emcucaeg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxsbxhv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wfitlzum.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vduupeuo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vwuizwcj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qbjuaxgc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtbxgpcm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rttyrxnq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2upgowfay.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ofgoqgcf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xunhpofu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xltoiaxy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2khfcpbrx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2nqargvqz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2spjgnvkx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqvrpupp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ahenpcac.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qcaqllvz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2glqjdlmo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mnftudfo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yvtlprks.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cfjggifq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nalxgopq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ninllndk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mszdjxyf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2axzzwrgj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2umqeitkj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ybvvlzup.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zyqxikwf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bhsnifxy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2euiqlzzn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vouytkho.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tqapccjs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ffgslteh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sbqsabbl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wrxoiext.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dhtwgmbx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2srnettbw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mtkzwglo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jzcwtnro.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vwbfpgiu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nwesiuxj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcgpnoss.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ujpsarmt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2krhxnsez.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wttodjlg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ddmlvrfg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kgqwnkse.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lufsjssa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbapbbfk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hfqmqxgt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfklgewv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wisudmro.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2enyukhqw.html


<!-- 参考信息 -->