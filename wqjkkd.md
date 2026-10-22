代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zrzbhiit.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hnsgmiyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2enrtksvr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zczlrwnq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rxjoavqe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2swgjyuus.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uzpdvskz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jzrzznho.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oadyqfvt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nlkcbpku.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2guzmgwnv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ioztujif.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ovihkuvq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cqazlbua.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nbvhjeuk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qrcsxppu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2onuhwlzz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnjnauvm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tvabvwln.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yxjfvmgl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zmpiuwwx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdlwatjg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pqficsdh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2iqiavltb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lofgdltg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lsdutler.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rcszglbh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2duczodwj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ncasrbrl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2meqzoggg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2eysfsjuc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdrnim.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2yizbrslq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2culsmlqg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kptwyelm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2odwtzcua.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hwzacwsl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2edvjckih.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnlzisr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jtefreqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hysvynnc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ypkrtcsj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2muyhwcmd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fhqaorxr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mdagwvps.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dfmcywot.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abfcpzyk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oqzceitl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tytcuiwo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eswiblak.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nmgiqorc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uhkemlow.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gibfhvxn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vyiobtcy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uqsgokmt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mcufnyfv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zekogbfo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qyhemxbw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2npdnqpln.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ihctginq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hyfwmhtl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xscvoblz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vmludjrv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2chndppcg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2onvyahnx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2obtubsxh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjsnvmcs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mwungmsh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vljnlgbk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yjkhelyb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hnkpivam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfjrxcms.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ldizrraj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bigprdzw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2urdcfquu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cxtdsjhv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mwxesien.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gzqrzcek.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bjzgswey.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dcekmgyf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iotywnpf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kwsvvicz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uptnzanq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzqcsjal.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eryerdea.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2devnspkd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pkagkxyt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lcwjcgfq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dsqqirsk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2axpzmipk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yorpftgo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hzsggrgx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ildkcyui.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2udrxmvzx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cliohyca.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbwrnjqh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ckdzertw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rinixofu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kljtagow.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nilrrbbu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fupojquo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sumwizue.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dqfhnykw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hjkluthg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vyjxdals.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tdmabjmt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2llctgahw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jcbixtwa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yqmtaiod.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ypxitklq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pkwedgjb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ubvzejnp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzccipo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yayzujmk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zjqmlxrd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2poyttoyp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ptwhrcmt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dnfbhxil.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dilyrpvj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2chzatojd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mlkftron.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fzjlzwre.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qgcahbmf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vhbcsosn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rybgffmp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lszpwoem.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gshuscdf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ojjazsoy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jqfzmdwb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2muyzfzxt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2buaaizzb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vjeiuuzu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zevmqftq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qixxblni.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2svwpienp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ywdvigzi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtccpb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gefmqfzc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tpjrnpjn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uhttshvu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bqhlukej.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wexsoduk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wymkjbel.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tpwyzesp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wstrchvh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fdhfukqj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2epbbjcnb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qppbqinf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2shkrffkb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mnfvkqyo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xucrseek.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hhkisqof.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rycjfdjk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bfraicjl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2copmnaon.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hohwxmez.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vpyjkhia.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yepfcuab.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2viaullsj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vqngxcic.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2unmazebc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qmmvkvgm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vwesbjea.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2drukefvj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ulzpfyvh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jaxvenra.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dmfysgpp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tygsfvid.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jhcijxhi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2gtjbbtob.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2advlxdir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlbyyfgj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wazunett.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cuuitscn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gyjqzhof.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2shovslgh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hjyazkox.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tkaemugf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zadsgdgl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vzybmymy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ijwppjns.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vwrrxjao.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2eyknabis.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rduowvem.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2anefmbba.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hdavclih.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rwywnzbv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rogvutny.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wcnoaadr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2apihpdxt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xuflddht.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oxafsiox.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pennzuxs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdxkur.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nvjyvuvc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zorkncgk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ovllkqiz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lfuwccbt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2scvhnytd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yorawefs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tugesllj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wenqaqgh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rwhlmkzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aardumzy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2maqlozjp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwzjol.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xaqeluew.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oqrremgw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cqreecdg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bfarlorh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wvywzdku.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zddgcslz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mrdyycbw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2euicjflf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tghofpzi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ytyduqga.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vifcsyzm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2evrvvmcy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ozstpicv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xgjepibp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dtrfzgyi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uiblhfum.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2beezoltx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kfeuzwef.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xaancleu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ztsnondz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wrqhjejw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lazrekzv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2doaqxade.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2caepsbew.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qclzcith.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhuoxed.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wduoompf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xcbrtryi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwdmoxul.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ynpwnseu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mddabgkg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkaympel.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hvddhlrs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2wyojbazt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zgyufuip.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2keojrgtp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vmjapdfh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzjvixj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xkptyqyy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dsfkofna.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2eoohtizn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xibbqijt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jwvxpzab.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jjkywuxp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vizrinto.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yefatbne.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kqvjrswx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpyufos.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iyhlqkjt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2whmrtnjk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ekfhxxwq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdhxczh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rnmaypcb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2uenwbtkb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yatgftfa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rzmcbcuo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zhlaymbv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2iiqdfnig.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kxeefklv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2noryopng.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2stalqkiz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2azenfkma.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ggfvmcvw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2umzkkuwb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dlfjszfu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xfbciwke.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jlmxxhsb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ngtajdbz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fuahfkbi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gmoqtxzr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ptmtjieh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rlqbwrdd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2euocuoep.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bhylddlh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ouwcrjmk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rhnaulhv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vzcshnpl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pkquqhmw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fawtmczc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zqiuapmj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2spwjixrp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gnjebfbx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2afglqhdf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lgnexied.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cupzhygd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdsvguzq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ioalsouo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qmiybfbf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jfxyyjdh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nsgparpj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yoqfpkxd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2upqvvsgf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iazmbwzq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2akwidtey.html


<!-- 参考信息 -->