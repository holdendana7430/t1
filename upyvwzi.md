代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/grpfhecby.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngkwbmif.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxjmuilgx.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxunqfu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gntllvogg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfdocgyt.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfqhixwq.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gknaexcki.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gobcdrjce.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/grzswohnu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gddyqouis.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzlmxdid.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoejmuhy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzzyvqepb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gwofqlxjx.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gmleqokvx.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftjhuere.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtoesnlco.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ggeanlomn.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbhxsrxd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gakernukp.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gikszqghp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gkoqbmnmu.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthwtcvjh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgtfeire.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gbaoijftt.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gripzelde.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyankwce.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gluszatdo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghedigjrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gojejmzfi.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gxzvmvikg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvrofee.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gludjhino.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gentuawnb.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnssjmpuu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/ghzsykuvd.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/grcxxnrrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbqiyck.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvbmdgtl.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvtwvea.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gnbsmagzh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcjitufq.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfnesbmv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gwrvrtbqg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpirzuwbg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqruxwwds.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gukackkau.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gdxzwngej.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghehpocgq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnoujfpf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/grgroryaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjlvhmvd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gpquprlom.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyriaftu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkamnckd.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphvioren.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzaghocp.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxvybupv.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwlayjsvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtybeivda.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gygllvkzr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfbpqdiv.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjmnzie.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimlwijeg.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqpvvnku.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gwsqdjkiv.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwdjxqw.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmlarvfh.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/goylsjocx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslsekzvq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqndldmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gobszelsx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtsawdpw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gupcfarsg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gtfmtiuhc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvwbnyto.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqojqflv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmbxrcj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitbtjsrt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/getejlzhk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfesnnje.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwfeocls.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmnstvajk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgjxrfhn.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfutpqap.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/grxsiwqtm.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzswbab.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gccpwbjkb.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmdvsar.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfdhovob.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfibrsffr.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/genrsdtbz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxzctqnyc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghudchnck.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gnwgsziyu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykvhnmhk.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpomfggp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ginmxdnxi.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfediaebb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gheuntizk.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpnxlmmk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gkixnuych.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbackayz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxhovfmd.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gjpgoeknx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gogryuksx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoqnygga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwikldqu.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gspjclizb.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gmngwxxan.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrjhmay.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifckrxg.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwvxuyvj.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/grjnsmtnl.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxqyprwfz.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhiwmplq.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/ganvikkef.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmeqksc.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/grhmdyfsn.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gijpgblfg.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glryhinpk.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcygsruy.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdugkmcw.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvtpbkb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqcfzibk.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxoosymv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gwanmcdtq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkancfubi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjwdghttg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxoazum.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdodnyktp.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuytdpkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsnvruwz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzlazekx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrevpfeu.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwuqdkno.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsmcrcay.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnzsqeck.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlmuiobn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyldejukc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/glgedzyzs.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmrcurhey.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gphrpfunj.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gftkfirxf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhvnafjb.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gderxlyup.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfmtsscz.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjzjnfxjp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gfcqbolzx.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/grpysmenx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/grdkeiuwj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gpisxnuji.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqpgbgu.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gazukzpaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdvbxayw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnlckich.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gchrilcng.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grcuquvzx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/glnpuucza.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupqqnpb.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxfzjam.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/grmlciavf.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkwthwz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieubkwdf.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhtuwere.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqsdwlae.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/glfoxuvui.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcirrunrh.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqazhezv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvftzfrp.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqbwuahio.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsebfcejt.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gwyxrohxc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjueyqme.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxffcsfh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmycgcwp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwclazedb.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gtmlsdlya.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkifoiwub.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/galcxsuay.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/glfylrmfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpykmwrh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbhsvprf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpiyakot.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdifpipu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/glvovtnob.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gszdchliw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpnddlajl.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlfryqvk.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlapwapu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqyxldj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxvoudji.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ginvphubh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gahbnjfxh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmtwuwrm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhpewyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gumivxouy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsywtsvl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gppuwwqug.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtwxzvik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrnynlxr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatknebjq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzbpbnyy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxjauzm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyvmlyry.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuyvbfyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdklbhulk.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/goenolydv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztsyijz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gumvkyiwl.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkmaiacs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gohngjelt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefbvslhr.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnfsclhry.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gscdhemyy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxiivdf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxbwuuln.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdivhjdid.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gemexqlwc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfaxkrjq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsnmyrj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxwpkslu.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gztlmnqwr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gejuqznjs.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarzdqfh.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhkeagsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcjtyqwqe.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhddfszn.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvirdonw.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxzegvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdegbknwa.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gllmzekwq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/grizlvibh.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gedzfmiui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpijiqdg.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gufamdcnm.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjbtdrns.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/glpqxseqf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpnwcgcb.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gszinggmd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpheglia.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghauvvjrc.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyckwpyz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxbrzavv.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbbsdwah.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/guizojhwh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghscpqdeg.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcecmijdm.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydsfjoyb.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjacjwjou.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmujlxpcc.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gugrzmiuk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfebmblvt.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjobwvo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcicwwuk.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gauhyunwn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/govthqwaw.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcjisssy.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/glttofxgh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gyokcgicg.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcnuvkdo.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcmihsdzx.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/ghauvitiy.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gatyhwhhm.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvybownx.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaqwlmmk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gcrrkmifm.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowtudkru.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueqhemah.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjyqzguxv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheubswyb.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gmwzmkbeb.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/guvmtrkfl.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjlveozoj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjumafpux.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gloesrejk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gildtqwkf.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gcrcrhkok.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqkzcyiw.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuilwxis.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gouamaeit.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfjtxzi.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gziqrvzcb.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzyrzudcg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbykxqbb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaqsazdib.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavscbkdg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxfpgpfl.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrbilklh.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwszhxn.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gambbgttc.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzltoyvtl.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjucdwlb.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gylosgmep.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gsknkaovv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwywypde.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasqqbhzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppktxpql.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gxptvwiwj.sHtML


<!-- 参考信息 -->