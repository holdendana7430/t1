代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gyorfsbxh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxazfjcfr.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/grqbnlbju.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gvwilozfh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gkcdhalar.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gskawlnzs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gelesinjc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gzugxwsdh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gowfijesf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gjtyiczva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/ggzunjiup.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/grjiwefrx.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gprrvthgt.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gmntadajm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ghgtjnenx.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/guvbbszzl.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gucrrjtkn.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggnomrhkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ghnsczdud.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gkfyqlmfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gvhuiusub.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gnweaxbpx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gvemmxogx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gtzdxodlp.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gnauzquyr.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/glgfjhmva.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtpvucfmp.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gpojlzrud.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gsvzbxvnn.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gwnfmchop.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gqclbiewd.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gqvxjftqk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gxnnukpcs.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/ghejbpdlr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gftwbiazi.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gibanduqb.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gkjlqxerw.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gtsshhyuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gdnfowcou.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwemxqupj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gclccwvhh.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gvodkgqfa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/goxzgukcg.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gutdhdusn.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gxmitvbeb.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gwfhglglp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggzixezny.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gwskvkvni.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gjzguvpwf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gnuuqyznm.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gilxyjthb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/genabwqrs.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gnbbprvvz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnxzmmghg.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grtucuwxb.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gufmzereg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gcagfjyzp.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/ghibvjixa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gtpmeiqux.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gxmxjfjdd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gcfizjpks.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/giljncpgj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/giabzxwdv.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ghlgvdhth.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gsxvhanls.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjgwofbmd.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gnllwtkcv.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gkqnszhvu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gvrkqfzyh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gsrysgrgn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gdnkodsoo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gucncwted.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gmgpgslwt.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gwwcnwhte.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gawitvtwc.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gujbpmpgv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gbntkdped.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/godlkalli.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grklavmrq.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gqftfeuyk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gujfptdmc.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/ghtnyfmom.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gffwpcxlk.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gtygaqbri.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gxnohxawq.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gdgthfmeu.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gjcyekzss.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/glnqeadpj.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/ggjhopmgz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxqmjnidq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gwrflgadl.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gnsyqcioh.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gbnftglri.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gqjyqnisp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gefdqqjpt.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gbrpjkilw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvedeiun.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/ghryuvkmg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gdqwrglcu.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glyxugnmn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/glahauklv.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gpqgxdwfy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gzeuhqwry.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gmfzjhgei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gsbhggohz.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gubkeuawb.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggpzmhssh.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gsekylptx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/giikpdeeo.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gyumdgfar.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gjiujdomz.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwbzeafgy.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpwwxqqtf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/glqkaddzv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gnugyxggk.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gfhhjprrc.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gjaqesugq.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/grkcqyfyr.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gndvrnurq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcwnzuodb.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gzzmqmods.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gmdksvhjv.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gwklehdgj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gqmlsqeun.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gigrndwbh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ghrvkriod.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gdmwtkqkr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gdffhodpw.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gvuotuxya.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/graohrgwi.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/godbsriad.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnsmwoqxl.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ghovfhquo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gndiomimx.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gyymnqswu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gkjgjjtzd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gyqsauhdq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/ghjryeozn.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gwbqckwqw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/ghvrolzqf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtyazxyyn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gffwflhot.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggkxhbkfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gckpxwovo.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gbuirhkhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gukmwcgoz.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gqjjccqse.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gqwhkgiov.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gpfevwqjb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gvkdirtur.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gmgokazum.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gsdzeedsm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gvhiuxrzl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gtsatlxgp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grgsgfpqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gweuhpqrm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gdufozqqo.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ggfwykkrd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gjxzhrpqp.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gjildkmxp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/girodrbbi.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gckuyvpzs.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gilqntzgd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/grkqkeuqg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gocwtrgmv.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gaxlaokrp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gjlwvlucz.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/guzuiygng.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/guniessza.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gphxyfpxh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/godyjgpqt.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gkvqejgjy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gtcxgcusv.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gbvdbuypj.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gvpfnvvqm.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gamgmqdcg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gmebbwzgv.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gqkdaaotz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gailpgkuq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gfqeajyfc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gxymkstbm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdldfksdz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gfngikjov.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geibuppej.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsnagxdsl.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdqwjsuwh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gpytyklkb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gxnwjzojy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gijvhuopq.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gqqlbquab.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gcippcezs.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gxqaqyiic.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gggsnmfbp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gcoorebdt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/grtbfuswb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gllvaycbf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gfqvboubo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gjearlkkf.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gmkdwxhil.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gromsybld.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gejuojrmd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gllhybxcf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gtjicitud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/ghvmhlvuc.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gmojzhfad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gziygvmmn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gmmwsymho.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtkjlihjc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/ggmxloead.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gnazihgej.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gagpaviep.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gyvngfrpi.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gcqxziglu.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/godloghoi.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdsacxhkx.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gcfplgtrm.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gvnmwxtue.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gudruykry.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjbcdufsc.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gcexsapqo.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/grgmhsyko.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gzztclzax.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gczomqlsi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gzpmrcgij.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gndpnprhg.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gpdlzzlih.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gjfcftdbm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gonpkcgco.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gplkhznnb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gybzaieek.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gpjmtjsnp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gchjewqab.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gsodhtjot.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/ggdahemtl.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gpoknvtmr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gvicyxlil.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/ggnaomimg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gtdwcrgfj.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gokmfuzfi.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gjrnalnhl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gynqcmhde.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gauagffiq.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/grzywgwwd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gbpimofng.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gxditaxua.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gllljlrqg.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gopkmzlkr.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gpukfnifl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gjolsnfnt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/goljxfwyg.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gwovyctyd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gdesctfdx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gkfiqvhxo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gqtyxipkv.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/glycyynnf.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gunbkqdut.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/glfqdpnrg.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/ghzwbbnoq.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gtgpeypid.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gojxzlvxl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzilhotes.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gaadljqal.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gieujjtrw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/ghduawgqd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwxsyexbj.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gswmwalzy.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/grfykppse.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gnciwgdsg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxqlevhwv.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gmtsfcrmg.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gtnugavum.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gyemjgnmp.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gjqlteega.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gnulgxlno.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gacslznsa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gpjmknyhr.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gywasuptp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gfkoslwds.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gapbbutwh.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gymlqyshg.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/guhsfrjas.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggloszzui.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbojkbfzf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gwjbyyrhc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/giefgxlfq.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gqkiouabf.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gplcigetj.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gwkutnnuk.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gqpbxiffu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjrtebpxy.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gljpxwhqe.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/globcohga.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gjlwqbgoa.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gnjksgkxq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gftgpisjz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gomkkmmvh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfdsgdfej.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gpmpnweqv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gqmnsdiqy.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gdrhjmggl.sHtML


<!-- 参考信息 -->