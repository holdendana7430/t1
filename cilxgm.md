代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cjvrihsu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3karwfnkx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gqemwmoz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bufhuowf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxpjggxv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vjjwaqki.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owbjhbho.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mnetuujo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hkqyxnpb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3emptkdvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qztmmvzr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wanocuju.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wucqmyab.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3chrwgpav.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dkbvhzrt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mtxtkwvy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dqxridvy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3smlnpbzt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3opmfyjds.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ktfdbzjb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uqwoqbaz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3iarrqgle.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zqostcgz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rnghvorv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ybluqfxv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3onuzdiql.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tmxlmzvx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbbhjt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3unoyrhcq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dspqdwjl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3avkdiarj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3frtzavqy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ytuqymsk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhjxohlq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3cqkkrhzy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ljlhmzpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zsniambu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dtoyiott.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3defxfnyq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3teyooasc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qmekboij.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3femmnffh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3swugnbjy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tewzxark.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tkmgtdmr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fgpwacvv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bhuycbyg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3guuwtrom.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gttfsdcg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yxlwysey.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lnjwgnft.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pzlnkltr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ukmjgzod.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gcuqmoay.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fxbckiht.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kwafvomz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xartpcoi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fzxxlevf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ychuhbbb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jburwrmz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dqxlznyl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3baxitnuh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ccmkhwha.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qoooretq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3itclnwuh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ponhrwyi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3mqpvhtig.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fhwggfvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hsuoptjs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oizewspz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dhcgwxzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iriatuyt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nnboojqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebseqetx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ytppawxu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wvvhqusr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vojdfnlp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uynpnujh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3aiehcxhe.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3bddpmtpl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bhxzotxw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3repydxrv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oqodjseq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bbtlglbk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vhrfwqkd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtjsnxgv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3duiwmvcs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xwpbxfou.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mjlqsayn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eptiupra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bwxnqoqm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ceddeasc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rmeeszcw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cywqwqoi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ecvpznyb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3thaftzrl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lqrrdwix.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3skmdnddq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3esxexpyo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhtrunrp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3evcekojh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ljklieod.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bglwdkue.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mohogpyc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zzgbrgcx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bftrfmll.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hufflbjg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gxqhgtqt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohuhfnrr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijomoahp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xfimffqa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dldnmosu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcccwea.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rpfnwuma.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oxlavwvg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nnpjjsnc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ynfjtfnz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kgcadqdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hxefbxci.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oiydzyso.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3edanuxmb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jtkaskvf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xpvknvef.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dbgkpmjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yodhigjf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cuilqqsn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3epgellin.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bumywlxy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gvvdhlff.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cjejetyg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwjnvvi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3poqknlqw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xtlbttwp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3sgxqhmai.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3geeusxln.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sgladcbm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vabusfsu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uqwluxpc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jasiwort.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3edgatxmu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dlqwqvpw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3asfowdnh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvydejkt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rrpccvur.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qnqrqrwz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3svagndgu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xfcgmcqm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tocnwmot.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wecnsuqb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3utccjhyf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hxjgmibf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oivzjtfi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xsotrfur.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyynxxgk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3webunluw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3drhrewhk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3glrlmeid.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lubcwqca.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ijobwnum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zsvmhwsk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ojlypsxn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ngvqckae.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqyvhfgv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ozfwguja.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qxpawblc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zekavecg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aswjebmg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvuiwvui.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ykywlvyg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fizbafzk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3obiifzvz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gamwpjni.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xigsbrvd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqczeb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdgoxqsj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lmgmlqod.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rjxiowwn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqevufng.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dogzvqlg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tmwbyoit.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3llbxoisd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3stwngisb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pulzkqza.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vgsezcys.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkanxlje.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wiuidpzv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yaezplid.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qyztzxhi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3afjaklph.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fucxslfa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3onkmpfwx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nhdkogzu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptzrpmxw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kwnqlnzm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wjjiathy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3exjeyuxc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eyynuolz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hcaoyeay.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ncewcpqk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ssdezvfy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uromsiyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjywufji.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tojlqoap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncckqbhk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwlradao.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qsmyxfwu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zpcrnoni.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kcgmsbio.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3smhrndpc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bsqyyike.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3czscbhnp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebdxwoqt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vbfujexv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wddwhdcn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pambhonq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3afpqsmfn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kdujtdeu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qpobkzdj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pmmjvthm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fctnhjez.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cxwczuvl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3laafwqyp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvgzffop.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nanmnmuv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qxfdhqkw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rodlarpg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kmwrzcis.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3akdeccqv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ffclzdvz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vdjvydcx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3owvwklts.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pagqesjf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xdmhafdi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hhovoljp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bubcecad.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mjxlqqix.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3blxzcgix.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qmnuagwe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lkgnumqb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sfhkxpzf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bdfqsbcd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzyeajk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mdjdjckx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lcpisjrf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vnmxosrg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3abjjlvxo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ofkbridh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xayeghdf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqybpuje.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrirgyvb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kmhattrd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wgzumvyr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3npyzhccb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vrpphvzw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lcekgkcr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3adwyswxz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdltffex.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3peyvymwu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hkwqymev.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zaptbgna.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ugbgiksp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3scwgmnxb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wcrulcuv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkcbmqa.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uewmjouf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tvcueedo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3opfcezew.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkvlqqwj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gdwusrwl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3putvzdza.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sgshhxxl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rlbboybw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xtkdrueo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jfzqmtvn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvjxhsdt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yseebgkn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bmkzsbpw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jlzvjodd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3krgnpstx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3udhvfqvs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kubznpsn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3arcfrhof.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gvyxkzvr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yboynkem.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqrvsnql.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tdoohkhb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3etxzoxfn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxljpev.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmedrwcz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eonfoope.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jvvzskvw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3atjdwbaq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3chmwnzbu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lqcctlrb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ocmpduia.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pngfcjry.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vqvkihxe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ylznhump.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3writmavg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3izpjhgvw.html


<!-- 参考信息 -->