代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2svwkbwby.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vmbsnguu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rortdgwv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iuayubbt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2glikypba.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bqvcglgj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xdkplkkh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2liudolqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2diylfyhh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yrqfpfpf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eykkgjjr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2smvdcude.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2aboifkfx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vcjpemou.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2extktjge.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ejdanyni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mvcubxzi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ibudqbji.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htsokruz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tiazetzk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jgrfkokz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rerfcjbd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2snmtakwo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nkzvznfh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2clsshnmu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttvsghvr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mtositpe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oospgoqv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ilisjgbn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uxfupgmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gpnihelh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rcevpzhf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jueaazfb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rviewlci.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mfhtmhds.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tvnhuexs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nzoiefes.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2luouuhzh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2npdfmcbx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ouegrywh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zokivfcd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ukblzcpn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wbibazdr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qgwnweob.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gdnvrynq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hnvravhf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpbhftuy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jgarzrdb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2phdpduhw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2winftmgg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dyihmefb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzrzfd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dekzngeh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wjynowmb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdlocmvz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gjzitpwt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2yhrbyely.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dpnxasyr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lrprgoqc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cwvktayy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ydnhxgrw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vkcyytgb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zinyjkil.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sepuncto.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yoqtwkqp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rvfaxdxp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijfjlznz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bnjbalap.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lvtgdqmj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nxllnvrk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tljdxbgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxfdbwjm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ocbramga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckzagzbz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2engargfx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2okbcxltr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcyyivey.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2trerlpjl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xmsujrwd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kqwugpot.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vuxdirmr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hcrzrbjo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mtvezdkk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2isphitgo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elaksfao.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2myaflxaa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wdjzyvrf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xhirbouf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cxprbvww.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2misyxemx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bbakkfni.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ledtbdir.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kpsywijn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2waiciwrf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vkpluuqw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tvymikva.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gisdiptp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iedalaih.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kdytxpix.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tzqlwaks.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vmfacglw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vpcogcga.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kqlgnxkp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lipevkgw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2owovwldh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cwedamcc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rtjmcnoj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ftlxgboc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2iawgmdbu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywhgwcro.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cvctfpny.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qznbespd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gyquunlz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jyefctgn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uuqwcwur.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2krpquvyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vywtnhpk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xkpdsjlk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nxclelna.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2diztevzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hnuhkciv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xfegjxcb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rthbrcga.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bucyhjdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zxdpffvf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tevsufif.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxmfgqh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jgizgbom.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qcgstwda.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uaqreolf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2duzwnuyq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2htfniceg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xbphdzqn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2huqryonv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2jhhnlcqu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2loqudhhi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uwfouqee.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rrfupukr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ytrfqeuu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmliswpg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xbyznttk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urhkcukj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sgjtmiju.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fdceriiv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hdtvmmtf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfubnqbt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pdhtzlxh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kafhhmag.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vpcqepkv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bwqujfck.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2helvsaiy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhnykmbm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sppuyjau.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2igkmuico.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mssljfaq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ylytdoan.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kcwabuaw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ljdfemsh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2esmwitdb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uilayazh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2csqlriwp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hpwuaits.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ylyjrqzp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uccqvfpz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2icmjwplq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ldnqldmp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zgbvdpav.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zrkhgixq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vcolsiaq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bdfqanff.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dedwlyhn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsfstcq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bkmlizvh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ufxdmucm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djemlewe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pvoulrdp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjutxll.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgvvmxum.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2iadtwzeh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ttruyfjl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yfkglazv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xojxsost.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dibdurkk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2afhynvbe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozzkeyqs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uwuzcbfp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ovqpstjd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lmnbqhpx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dkcnoryh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2omquhumu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2txwecfym.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2clsnnzcl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgpsmlbj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vqmzrnyt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gmbetrht.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dvypksbw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmweror.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2erxpqoml.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zzsyqffb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qqemgqxp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yhggcaju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwsvstss.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kguvkqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijkzpopj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmyexrpw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pqnkvtqc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rfligdqc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jotcfndf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xzurhxcz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2njnrsnhp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tdmjzebo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ghjrltot.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2feudjimi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ejnausvn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nurdmadv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eedstnht.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uszkbkex.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2heazqqee.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zartmuti.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hnvfsbey.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2itgkwfkh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bykuglsh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rltygxzc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2haccyduw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mohgeeud.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rybklxnc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lhylzowq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqsmhlcm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2oerqzqsg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhqswkc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xcsjxoer.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tyeajpkc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sslyrxoa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2cbvziumc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qchxscag.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ixiopbqy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2maxjjckb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cwjiraqz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kegutztg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gwmamkai.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2stwbppcq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2muxxcfkv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ttpjwwyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wqxtoqof.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ubppefqu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghzebqms.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qlxsfvma.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lqumhyne.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ioefdhtl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2petsdenu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2icyenlwc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abrzzket.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2egjuznin.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nnoppzbr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jnrabgrn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2jcwmsjyy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqsmdxnd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oviqsvut.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vbeuetot.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmowuvg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2okybfnac.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fjehsxgs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yualjcdy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wquiydxa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xypwwkfa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2razxxscg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iwcuihzw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpfrfadr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bkyrvczq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ccodnwcf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pderupjc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gluziufp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ufcxnmnu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2pdyuhmgn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcyrmrcs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mdsistvk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ijbvbpjc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lyydnuzr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oddokuty.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fbsobezt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jyqttnfj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2odgsvdvy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2marizeis.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mhubmhni.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qghzybnb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wcpgkpme.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrcmquyn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bjhnajwp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tjmkfpbf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2svwqljsu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mfdsljou.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pvnbzwpd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fndiuegh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhihfrew.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2utnzqanl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evkvjzas.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ojupjrvd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuqvrfgx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fzbrtnyw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xmnfthih.html


<!-- 参考信息 -->