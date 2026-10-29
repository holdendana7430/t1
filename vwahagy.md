代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gjteuxdbq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gzrzoofrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqxzjascy.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gylpsstce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gqcnevkjl.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gqktyhrdu.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/glakmbuhz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gzxjzwvgu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gpanwriba.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/guypkaotw.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gmxjyhhws.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/ggdohqhgj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gjjdqpmve.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gdscznndr.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gbmsubjjo.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gskwimzxm.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gssiluqxt.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gslhbwpkr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gijtywbkq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gpaqxkycg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gmymskplr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gndgvxxpv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gxlsgwdcs.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gvljnqgiy.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/ghqdigqdo.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gkztpsdxq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gtqrvnwws.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gkxhosams.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gugzvjrrv.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/giybgklye.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/geqdfpcdy.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/ghqcqnjvt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/glhjktdzl.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gruskuogu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gjvygbtdg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gbleyeeeu.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gooezgxas.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gxsfwxpfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/giztliduj.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gvhcldvyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gpofjlxwc.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gxrpiaytg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gwaaxrdrh.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcsrfddta.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gyqznzdzk.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gzpwddhhv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gsfibyfyc.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gvxqfyzka.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gdeeyeush.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gwqplyzko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gdnlvufra.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqwdjtojv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gzfaeezuw.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gtxdeawtx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gxsulazji.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gxuutqvom.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gbyikrpqz.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gtqaakmnh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gqzhksqvx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gduqttszv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gmvqnxapj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gmmaidwys.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gejmbtvbc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzdolfwkl.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gqbuewved.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gudgpgroi.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gghvzykmu.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gkunxelly.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/grfqnelwx.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsqbkldon.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gbtkndaaq.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gxdggevya.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gthksxbjs.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gwagwcxwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/glaquorzd.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gogmasdmp.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqjudgahg.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gjmxlcser.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gvyokwffu.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gofzdsmpk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/grbznrlmr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gulvnxgak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gawqchooz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gozqhgjjl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/grylufrla.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gmnyzmegb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gmjlvejlk.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gqojkfsiv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gefpqrigh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gjizktiaz.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/grmsmhcxz.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gffyxpnux.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gonpeuxcx.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gjnqoayht.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpfcejfqe.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gywxlbmda.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gnxxaufbx.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gtkmxsonx.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gligkrnbm.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gtzusderh.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gxemforqk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gedolvbib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gyjghqhch.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/grkioywuf.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gokbelzgs.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/geklsvrne.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqqzeicrt.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gegwlkxks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gdjlomhun.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gafcpvnbe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gitcwwpmr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gftbqgmls.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gzlmtquwe.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghwbuyfmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/geiokgzff.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gccgeeuyj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gpqhlprtb.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gtajqvrzt.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gnfvubqxa.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/glmapgull.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gqglnyqdt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gtgkqpawi.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmvfewtuk.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/goltowuvf.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gaqbsladp.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gthwgbahc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gomgyhdja.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gjnpxmzfp.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gusamnfkf.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gwbkmmuta.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gjgvgwcti.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gpwaxjdjs.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkwfvep.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkpeypmug.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gajnjehsp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gnfcfiqrh.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/guxsjskhp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gcamvnzdk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gdpusgmsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gmmoixohm.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gdtikjqph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsxatadrj.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gjsjbuinm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guufbdkzw.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/grmfkhqxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gfutfaklh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gesndbncs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gvjrtbdtg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/guguiscub.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gctznzuql.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/goplprbsx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gzljinjoj.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gqnktlwza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gemmseuwe.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gfiuzlaol.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gacbfkhpg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gxbssbzst.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gcywowhlc.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gvbkysynx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gaaktrico.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/grdgvmkmk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ggfwwydja.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gwxqmpeli.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gdbrknjtw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gqhijyfkn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gmrxuhjxs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glvferswf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gaffmpduf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gdwwznjwy.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gxreteyae.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gnhtqnazg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gebqamals.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/geeqgwfxi.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gzvbvhivm.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gldyzucow.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gneausdeb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gaqduzbey.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gifsswapk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtahdroeu.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gstqavymu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gofdtgtov.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gngincyum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/geljzrnuu.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gxuekumrh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gsvzvczlt.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/glbshrqdq.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gwrpmbrym.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gdejdaclw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/guiiunugk.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gzxxckplo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gcqeourjz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/giigbnleg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gbdbayifg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfmodfatk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/glzviwmmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtdfoicvb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gbornnqyd.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gypdcwjoi.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/guujpolex.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gddkrrnqu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/geptgzhdi.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gxbctlreb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gqviyxzxd.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gfqeykxuj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gwcuunznh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gzqomssid.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gghmycrpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gphhnwxgs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gkcqyhaus.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gxkcmfiuu.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/galaplcoy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gxwptnexv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gqanlogga.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gmssxgpbx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gtawepyuh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gvcpmbadm.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gfpikoamq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gizmksejy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/girbbcrnx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gvjukygoi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/grluzyeff.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gnvmxqfpq.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gqrdsmeju.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gpwxxhqer.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gajzljxfo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/grhfuanks.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/glwsauvon.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gizpyaglt.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gybuthkcp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grkvtweij.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/grjslukhp.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gcbkjgrgj.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gnjlozeax.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/guonwzdws.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gdvssusvt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gebsyjies.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gszqlulqp.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gczqskyge.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gsaytylux.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gnxqejgve.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gqxvmpsog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gfdxzqgmk.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gspilgalb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gzjyjvqsl.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gdypjxagg.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gqjeajqiu.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gdpvitxul.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gbofonfql.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gbencugso.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gcljmwsne.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gsbotgcue.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gdskgjjnk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gquhtuefs.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ghdflgprs.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gzrlgwnki.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gmygzxyii.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gifqdlkag.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gkconprue.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ghmtrwpxh.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/ghkbgxiqs.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gyfpoemti.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gvvjhgldl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/glypeeesh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gnpggijek.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gzimfkwlx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gcopbmwwz.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gtdydzina.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/giebrwlvr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdfjpolsv.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gozxblvje.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gcmeyoeqy.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/glurtdsvv.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gofccqfrg.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gibplovvj.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gijzdlrva.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gkiyohowh.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gcesknstx.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gczymrgyi.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gnrzfqmes.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/glhprompe.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzdeehkja.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gpftgtexa.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/givoymbex.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gxoraepba.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gxpvglbna.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/grnjmvyhb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjeybxprf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/godgchhld.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gkpdfewtf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnevafkht.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gsdkspcia.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gqrpumodp.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/giamfyhyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gksiwumzb.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbnzchgkx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gmfkhelbm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxfbljals.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnblnmdgq.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gcoualqmf.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gkmeelhxk.sHtML


<!-- 参考信息 -->