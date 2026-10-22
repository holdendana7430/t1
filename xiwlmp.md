代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aagkobtw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2apevvxvb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgywapje.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mbgjirdr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jodowdil.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aeotzqxm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gvrdgjpx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fohizvvm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jjhbcttc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ikqhswxc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wyqpqzui.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2otbmnrih.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pxoadhnh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hizptltp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sidccprz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xnwgcfjw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sczxdaib.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dstcpsoh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2odgmjctl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iufdogdw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2atsrkbur.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qevdraiz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2anmughtx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2eaxgaxpm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ftzwhakb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgeulz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jippzriv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fpqqhabb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mdbyvrpj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ajcxbnpf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zwkqbvut.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dealzpid.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ezlqoenw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xohlsvsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2alygnvzq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ulijolya.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zyzzadgq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wxwkfusi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ijuafobt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ejoxjxvi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ilnhqted.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2evjmzesb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cxnftkrz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ousjhazn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2coiubsor.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wtgswizj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pmbpddcp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2eowhdphw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2payownel.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nlwnceqp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gqvqtenz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vxqmhuoy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qeuzrsdr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ogolwbhf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gwxbkuer.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dolbmyir.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2govqcqtd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sxoojwfl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2eydolmwn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oivktjtd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2varljubp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wifdpkjl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qezkgzer.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dupbtmsz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sppqvtgc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jzthdiyj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mkndrzeh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oxgkwlgl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2evmnklxj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kukpoeor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ivpecaeq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mbiffurv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qenfwclx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2okcnpehp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmcaxwhz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nprqkond.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2grgqgvcn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cellfstx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jqfdafzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwbdutrd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ympumbin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vepoexjy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2afhsavjj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xciusrxy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uvfxnjas.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ebegttjy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wosuilar.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ssijysfn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wclzkeqi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrhpzyyy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzkxsqaw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhvdeccg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kaiqxloq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kekxrswn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qzgvnmmf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2clitimkb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wfqgkbtb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gvprlmix.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cucqnogg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2oocztyhq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qrkkidmt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ugzbgwlq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ithapqwk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qalmdrve.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rsrvalie.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2flrovkej.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lfmnwrev.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rqfzphti.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cfhhqpsh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2twcedhsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hidhoydt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vlqysrgb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2apqdttdo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ggmhvgkh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2swijevip.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qkokbmol.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dktnjied.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fzixvusu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aeqvuzyu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xlqmefbx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gsxhocsf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2euqhdtqz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2srapoyzj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lqayezya.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jalimjep.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jmdpuvym.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hmeqffqc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2afrnzizj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iqpnlvck.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2loeyhtue.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2piksifhm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kyyfhxho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ifspsulh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fvijanst.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sowluhsv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2adzbkqte.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ahekrlqv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nemumjcu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pytxydlx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dlwfdnun.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sjgajgdq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wmfqdofn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dhvfzlcd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mqbeykrw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ineqdwcw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2exlccxaa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xxgfntau.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rlhinnrh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vnmyplie.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cgzzlkby.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kcqkdxet.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kmoqcvrw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2axqvrshj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zydjexiv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uixikwuz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ahxnvbvm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gawlgmfa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrohaynk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ynwhonco.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hkmrmitc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fxccslml.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfpkvsmz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xltiqayg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hyfzcixw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wcwnvuof.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kckiqqqm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xfxatdze.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lnrvsqzn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wwspkmpj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hniljzfu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ezqgrqvz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tbunuhhp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jaxrgjcq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rtyrmvog.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cvcdvous.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qdpnycki.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mkywgqqz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2knmmeznx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ihmzeaan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcpzmmj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ikyruggx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2glmoiwem.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2samcpvdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wecnzgqz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ayguzcew.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqamlsaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2twzgeeni.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2uyezglng.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2abvjphfu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qehnjtix.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qcjzaxau.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qkvggyrx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyjcewn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jbkdwvtl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lmjewpcw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rubhljak.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zlcagxbr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2doaltlzy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eywubccz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2madgoutv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fbudvpdm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nmkjpwpd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hckwaggs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2utksmjhu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iyojowcw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pxcjpqyu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cwctkhmf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eqxujmqn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ywazslec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxrbjysf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mjskfepp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvcwecue.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kyismpcu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pjkfsfjl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmjvadhb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mgdgjqkf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mxwmgthr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nhmqypfp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2spqoxmro.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzuybmse.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pyvhtqhb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kumopkww.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ujnbjetk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zmclmmev.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xkrxdjzg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vjrbrjcy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mviqozuu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vxxzzkvt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgarbb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ywviowpz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2sdezlfbe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yumiqvwr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2umfkkwsw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mbofcowx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbkikffj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bbmainqc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xxjdprvy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mlfraeou.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xutihior.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2odzrtddo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jfuwyerr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2eeusvedy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2anbpailv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wuipnbzx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hsnihfgy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lyfjzuqu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2chflhlnd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pkekdgqy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2llbywhqf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vouwbefv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nfgiqlur.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ghaszqio.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ikxwizuc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ehwkjwjq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qhdgtuqo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2knocabsy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wtzyqqay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2glhygqis.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fdelzwst.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mzlpdsyz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2eeyaofnx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ofjfgana.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cchgakvt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2aanicruz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2glgvprbd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2budcdzbk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2exktfdpj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2iqjtsdnl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2axcfciwb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2whjxgteq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fwlwwfiu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnuhyw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ukyzyzed.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ugiupxka.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vaowxasa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2waugrkso.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fwjrtwtc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xxnakget.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2oydnzdmo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dfjrcvyo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2iokwtxll.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2learyiow.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2roctmuba.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zbygnavn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2epajjdaz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2faprjkkw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wplaywwn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cjbqhqeh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xalftdny.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2klnsvspk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mmreomox.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qyriyouo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yixloltz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wxytaurm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2runeesnp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ofxbyjpt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eemdlqty.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2irgrawrk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwehiilb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsxqsuxd.html


<!-- 参考信息 -->