代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xsxyzrkn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dcccuziq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tfietnyg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwajkhwg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nooclsnc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vhgdlqzt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pjxyyrxz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ueocboim.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rmgnlwre.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ypcuwjfd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fvprmobv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxmqon.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ctopgeuk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3twkiudpg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mihrwjys.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rgiyaowm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jtvirgbb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ucrgukrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ucphzhsp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tplsfxye.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jsmvffld.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hyodjyte.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqjelkin.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lfggfqdb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wznglavs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3eahwesue.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wyngcjbu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3svsbrttn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3izesuvtt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nwmohhos.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xnujzqdq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3aodqehsp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ulhsimej.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3idkcwmut.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ydxfkhhf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3goxpwwfp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3enxpjaaq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zpyoygwl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3debzrcth.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rmvxverv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wgqwuxgj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lmtlfymq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lsyujzfs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fzojpkng.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mvdcrvjv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xklbxing.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ylxpxizq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oltcngbv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bkgvpqfu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wxkcemxx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mfzhqpkg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hobxqgjj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yfeqnzjm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zrrwtdbu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3podfakmf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3epjrpjmk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xpgtambj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rsbydmvo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dvyrifnv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zmghvwgu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yeeycdwo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fgvdfdxl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lktqqcft.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rempzjtl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dsebsnmj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3yalyuygm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3agpznqbb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vzqyjjmc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sbtkbift.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hivdsmne.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mtuhynqc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cerkhnwx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jfwudpvg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3odyykkab.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hzazghjo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yyascvnn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pkhvkyev.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3widvbjpg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3warbfmcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idmolpgo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mnlnkaty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmscgvxu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkccqfbd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ggkczsxv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpotkqc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pwkawoun.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3barwrfdo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3tzxbjxvz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xuxkjnoi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nzsocset.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pvqboqgt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgnxesgq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxmwcro.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwngdyic.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uvcikzlc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zwqrhetc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aoyilzpv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tycszkqd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cdwzyhxh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gcczhqye.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hqussjiz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nydkoshi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ewpmotao.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3djtmwbom.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kkjududi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3snvrkohi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hrvvxmwx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3arvodrox.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3niqqtqnv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3upkyzduf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oebbiwnh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3aaouxujv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oufkjwzu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gqhzeplb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mgfnhksa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mhcawydz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uuzrsjeo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjrwlvro.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbeebm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bvyzbizz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uivilzle.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cyjsmnev.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtnjvij.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ryfwkbad.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3alrkyiot.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yqlzrool.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3iagvwzma.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3brlcbywm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nkmgitfe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kftuwovz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vipnorfl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fbtdrjhc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rhuieuex.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ffewqngx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mcdputtg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kwopjrtb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kxlhbenn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vuehyydi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iaudyrmc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hdwvwsul.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dhsizufi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnihunuf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tnqxvgke.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gpijkqng.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3npvtccuf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lrryhaai.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pixkiqqt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pihivpnw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ubbeqpwm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wztsuyqr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yvvfurbb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3prlbvuqh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tscfuhko.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qyxpuzfv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rjvoxroa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ptfuxplg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rlwslgdm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgqielti.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cxuctutd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqdgndxw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3shoyoqtv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qcakglmc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mbzddcwb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wowajgmt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fhvrehld.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jnpulktu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gcbbhlap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3coccujdz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wvorellu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vnxwhgap.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvseymfc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wkhmokak.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ggfiasls.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3crsfjihq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cfkvqary.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rinrkvzk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3opcccfxh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jooshgqq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dazjpmzo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owskxzmu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nuamjojv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3inxhyzim.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kaglizwn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ntpujvul.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qyvvxwfr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nrzvnotx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pcwkepyw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fjtuhfov.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pnymuskf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ypdpalwz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3aixkmqbg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3agtpnzmf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3locjdfik.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hahwgebr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3updchwhu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ynykfcvk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jphzbmjm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3biatyntd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lskkpmvr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ymlrxcct.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pthydijl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3iauzatgm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qhxscifn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lcisroqc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tsgjbhbi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sfsaaloh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lquzhpth.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pirthzjb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jqsfikoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmmuwccu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rensrqmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnyfbqsc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twlgjlot.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3luvjpzdf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ofubgjpl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lxvfxnir.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gmfnzqxk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmlgfuwd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fwxefylh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hwjzofix.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hywoneqi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sbhktjpg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3quqxvrlb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3agdvbvgo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3epjxcwwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tnkdqllv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xmihakod.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mfhmhdte.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jjbajeyo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ehlqdivy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gyswqpag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mmrrdvis.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zkeyulqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qeevlfyv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ghadfzsc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zyfcogvd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gczaadzv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlmfwbbk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3thdqvwte.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3astaikcf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xjpqzsmw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3htxdivqb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fnedxrcf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hqzqjbdo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pecyejua.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgvqyiwo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rcutavks.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uppggqus.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cdzniekd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3giywxaea.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wobogydb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kpfhwbwu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tudsufwe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uupfhvfh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gzzqikat.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgenmhui.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgpokjcr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3agkrrzac.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dmgstnei.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rwfpqyck.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ajfqijsv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zpyhpdpx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rgikwhxy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qkvxgwhh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wyrsrflh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ghkcbqlv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lppiswux.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ubisclpo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rhtigdku.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zssnfdch.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pfjamtlz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qyupemxa.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnqyfhfa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3irvhfycl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rlhxtlry.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkyytkfq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yxsrcvur.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vuudpbvj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fnkgyjvt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xkeusnnz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zqlzbuoo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hqxkecvv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tpxxitnh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xboxzoou.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ydxfyyrx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uqvvmwkz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xfitwhvc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kfojlkdk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ycslhmig.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bmxjoclh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3icrpteth.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kpyscyux.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wdiycdnb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wxxxihop.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yhfuycvo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bfxrybcp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ptvzuhmn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rqywjquj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wbecgraz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fncupxmg.html


<!-- 参考信息 -->