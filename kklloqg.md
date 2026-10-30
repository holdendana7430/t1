代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gqohikigu.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gomwfxnwj.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gjqkbrtqq.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhsesvcz.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gcllnzicm.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gquhaflza.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjyqdcmzn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzmeiqmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpveiuby.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnfigrjf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gmefpsqmq.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gumzuuvsw.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gsrdirnox.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrgokfku.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvkktxfo.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrknherr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/giavezpie.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/goeoqcxea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gsffeqoxy.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdzplyvna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gtakywpzu.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gozghasuo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnyrxwkb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gpkwkbqct.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gehfusxac.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgicbng.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gicfvzwpb.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gwyfwqgfh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/giuizzbqm.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvatgmd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gaxqoecvt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdhlfymu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjmttikp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwhfxkda.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjchduas.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gllxqonqz.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbjkfoxmc.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvxjiqrqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpobkmshf.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnaywiego.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxpdwlia.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmusqyry.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmaejoni.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gsonfshhn.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gehmyrqvp.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gehrldlgt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxsvryxtv.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfgliish.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtlsbkyo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfilutacf.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwxrqqb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjdqgcaj.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixtjdtgz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkjexnqi.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcekummns.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gyfoltdmn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpspuisjc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvadhieul.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzekcjfm.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/golelubbh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcaerudx.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrfrgxqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyytjmmb.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtmuqeolw.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaiwtont.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrirssia.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnaglfwm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvdvbuds.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjjhjpnm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gjopdxogb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnijsaxdu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbloujhpk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdjnzag.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcljroqlr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeyrjqty.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjxiktef.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gpirxbgiu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggywbwpnz.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqrrvtsn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqsphly.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkmzzbii.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gbiwpqxqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwryumbno.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqaxzar.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gvrnxspww.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdudalhbu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuabtoqr.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gkldojrxj.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukvdcsmy.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gofgnyyea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqztrkoa.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpiffqed.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkydlcpg.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grjnhsfbq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjnlsvi.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/goxlwdsoy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxlizgu.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gyfpoaenc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gijfozhjk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfzsjromg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmtzzqyyo.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gadhewkkv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjgcyhc.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyawupxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcslodjt.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjcooyew.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgoptan.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzniwtkr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdoupmwa.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/grurtlcyw.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbaaaqhmf.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwpgfyir.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcaxubh.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbrzatlo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpjiclge.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkkeossz.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoqblzzv.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gehwnwdzd.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqbqlypc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdusfftf.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ggfechmsl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkvhadeli.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnsmmdylu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/geipdxdrl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfuxzrcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgvepnnq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gdljapfoa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtssqppe.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggomzgprb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwcnzbvd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdjvdjbm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimzzknxb.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gturqfdlq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdasielkk.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkgsrwja.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtockboob.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwhkjvtm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnugsyxvc.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjovcjxya.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkloalhju.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfihepeb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gezivyunv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpayhwbg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoiszois.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gccujvdpd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gyigepqqx.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnlkfktu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotrrwwxp.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpxiwkhr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkmweix.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/grngibzrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gctibubcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gsjypbgto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtflhvexh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxnbeqwf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxklpzap.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrmkhqnu.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxaophtzu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/grhttihkj.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gdpbbiauk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhglmhxf.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxixbernt.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/ggjfowvpg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfoncls.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwzzzoef.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gqhvxdfvv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdulvvwh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatyonbjv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjtfctls.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazucmcnj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvelnvwpe.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwzhace.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gevckwfej.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghelmmgia.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gklruoocp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhjakeup.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzztzeae.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/getpnvgee.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzbqnise.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxizufbmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzhfggezs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkapsbiyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gglfgcemv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaacjxezi.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gffcetvkh.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/giaxghgew.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxtpnrsy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbvdvyp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gsekpbvvi.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjhmnzzx.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gjbmhladm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhddwsw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gudrwrtiv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrvmhgyz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gjxuufuqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxtwpwcmv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gltsmcywp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzignzxlo.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gphxsfnka.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaxaqwii.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjhrpazn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gwfwjfblr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbgffmnkx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwqroqz.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfqnfogc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcokdtsb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsrbvrlm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzasdrxbv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gahyuhgpy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpmnoxv.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gndnrezmn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaicamqq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/geewzzywk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlmbjhvq.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnsuvfviz.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gksrfexhp.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnfrrdgs.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/grdfftenk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlbitfqc.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmyoqtys.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtnkqcog.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcflqusjy.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gevluagki.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwgznht.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqvgvba.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaimjbxjw.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/glyuzfhbi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/galxqaptq.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjpnzufyl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiziedwe.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpsotiy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grbsjxcuf.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gbfsesvmg.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpqdmhef.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnkjqiym.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcvlluba.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyivmjlmb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghwewebcn.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gzlfzhaki.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkgnochv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gfbpksnxs.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuqqswrb.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/giwgauhuj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gonynmrru.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjpkbhpe.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gejjnigbf.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrpnouh.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gerviokie.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvxntrnk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohnozyn.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudjfgjko.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gfrdtoytx.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gptylowqy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggihkglpr.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goqcaolhn.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gacwabrue.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/geilbyytp.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmlkamidb.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuflerca.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/giyazyusf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvxrqhte.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswpugug.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gprmsrguv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqvzwmg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnscyefy.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsdbobhq.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqyzywcu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhhtxxyq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhyqxhzp.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gqngfhhar.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/goagruzxw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaxwkier.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gppwlphxt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxumcgdcx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gizcwlmlh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyynnswbz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gcsdsexsu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrsiqpmc.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdoizgmz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyaunbtv.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdtfsdfns.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnresnlzi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwwvnyqe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiltwjjc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsphtqgiy.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gglfgpqvx.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxsncdv.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrkuxxuz.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghazltiyu.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/glmmttexj.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwwdiyy.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gbstfofzk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gblpcqfae.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsolzygnp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvmqoqff.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvdknrig.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnztcblkj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gkeypetku.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexwvnjgt.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gsnhahoru.sHtML


<!-- 参考信息 -->