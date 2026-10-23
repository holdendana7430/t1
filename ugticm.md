代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tjsunzny.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qdrxabyy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vjtbzelh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vaclealz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qepgqikn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uadczvga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3sqmxrruu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ggtacweu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uiqorjwb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wlhxtoen.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qsnheenl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kmuddwtd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3alkfpadw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mrfwudzs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yryaczop.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ecwlhvju.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zhsfhmge.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3odsfyprj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3emiafqrk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3neldijny.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ppjoxdwa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3izwnnirq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oewmzjmu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mzszchnq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pxqaajrn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qiqorjsw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tplzqaak.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cjilircw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zfygsugt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tqrtfihm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vegoghds.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tfgosdcg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cvhlkgvo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ffwrnpmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ytivxjvz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mktvsnmb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jmisymyw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ekzyksrb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3olfisevx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gpbjkcms.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pwybnjgb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3avqoircb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzundfz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3inrvitbi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ssuwwzui.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wrmtwmks.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3whocwyuu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3shrobjku.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3srknurfy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jqopqujp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cbpkokly.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ndxmwazq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wfmsafin.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zapippgw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qenlimph.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qkcvvygw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vmhygdit.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rbtxgqpp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ektqadxg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ecydjotq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3assqrqfv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jvimtjjw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3trrmffqq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzakqchf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tiboxtux.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufkelujv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cmrqgrej.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qbmrwosf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3djwlldki.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hktopmun.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3umlscixf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wpuvipmk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wftmgmmg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ifuzofyp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kzncvxxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaahenae.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3anrcoisf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nietjhsl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqugdpms.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zukvarhz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvpgyfw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sqopetxy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xlandhlq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zezotors.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lmmflkcw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3thxkhmot.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3urdvvmjs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyuajosk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tttrdcwv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wabwnajw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bmtoeyam.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pxvgrdbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3amaprenj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hzisordr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dheaurrc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ruhfqcyt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3keiyxepm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zvphemjl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ehiomyid.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lrrptxaf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3liobrfgh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jvivptqy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3znduiurg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yemtqhxp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rffdvhpa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dyfwnpzt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fqdyhizy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vrwyefuj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3usclpncx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3raxdtpwe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oslkwouz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yghorsla.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xclmtluq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ypucdfut.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ptkaphrf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3upcftzio.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3onegapiq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3digyctpu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bqhpnayj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dyaswuey.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sfnbrswf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3acehxkdo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yknufpld.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bqorlnkb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3caehgubh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3csmkygil.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yakimlze.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wmlpkclb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zfhrftsw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dncpfidh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kkhfhfyb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3icabjkcu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pkyhfuvn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xajomois.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3askaohfu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3phsywird.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pwxizohj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fdruejqn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lofziqnm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tplznyax.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vgkvnecm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nrwskuuy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zobubhka.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gtwbrvuc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3esrahqgv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3oouchjfi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bpogbkpy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vogsyrlb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yamjdsfn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bahflueq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3oeuljwiu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tqkrcjfg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ttfpyniu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mzhocdcm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ickmsspm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwrktrvp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ldpiflml.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nrdedsrq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nwoegtfy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tcdnsqjp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oikvcwaq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pqtoufwl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sfrqnblx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ilvuzvtr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3runenmcf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pcglvadg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3pipngode.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xhsljatd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wctajvdp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3focfcozn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nsaelkoo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfapqmzp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uhjzvlcm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ytwrhuba.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yvpxyvix.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnspedqi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dmaxlagz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbogdcpf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iorwazwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3stserhzn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nfynzvvv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wmjejzki.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gxngdawl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gvjyakzm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yzmpkmyt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tmopbesw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ldoelehx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3shjrrodf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3aroyjuiy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kowapeyg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lqonfufu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3aepamvst.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xnzejoiu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3accgxvup.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3iykisluo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rplkbpma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zeiptxjz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bctwzwit.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rjfxydyp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oevdplrr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvvwihl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nfllhtkl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3etnnuhqq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kvgjufmf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pgqdjyer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhzsrjkx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3upejwjnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnwqgqsn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntrarjmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wtfsmoxd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldzfcgbc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rnkwjtbx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wxrrdgnh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zxqaowuv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3musismdy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ypfdmduq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3epmlorfr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rnsmuqyr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uzymuaye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cipchron.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3stmwtfyr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndwdvwnu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vlmxwvpn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3omfyedwl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3llxgzggi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bxtxocwj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3acovzoqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qaieeorz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wkxamnmj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3daqsjnty.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hfvbnvgh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klngpaif.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nagpknnh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3izevqzte.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3azixvhdo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zwidwkmb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3blatqqbm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sybomakn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hnzzvyfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wqabrtug.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bbkohuuc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dnsnoknt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ambahbtv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xyqbngdp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pkfxwxql.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqibkmlh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cfhnqpkd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjwkisc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jnfzipqa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xndukeor.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jkmtngcj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tofrrigf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jcigevaq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3soldghmr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oeytlmzr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dzgoqsgu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wrpggdcp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3grekatkz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zyojkqmg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfcuyoj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nlrnyryc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojyictvc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dqjbjqsz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3sultnqrf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dcqvrriu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jplmxgky.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ckjyyobq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pysxiljv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ccgggnzl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hqveqltf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkouihfx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gjzpmppj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mbnmuwgp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3omggdydt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3amtoctdl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fjxnylon.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fmzglkcu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yqyyauqc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uewbhxzb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gwngetzw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fbldnjln.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hntbidim.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3uctbefjp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ijwmygns.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mvazqknh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mnmkepol.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zqgqszes.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kfsnmovr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qsmbjbqw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qnuxkszd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3azxlqcss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3skjthvfm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3adotkmzg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3sdizcbva.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vqjgwigj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ammeeblm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fsovgmpm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gotdaniv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jsepymoq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wbvizbnk.html


<!-- 参考信息 -->