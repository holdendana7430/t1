代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/ghhrybwjs.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gewhcbiod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gustnjwpk.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gqaemzcik.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gjxyrqyik.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/grndtdjek.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtolowfxc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gyqoxhjvb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gucwsijmo.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gyhkakojo.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gflofhstz.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/goovhviil.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbebtlnom.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqfohgets.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gxkacikts.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gncstchwe.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gbnbluxyk.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/ghgnhwdrn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gsgxwfgzg.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gpnyabxsz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gkknctcjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gnldbkqbe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gkdfbsqgj.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gquvnchoz.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gfhshwnks.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ghkdpzwco.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gbrblawvo.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gnadednmm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gsaaajhen.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gtajjwate.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gvzbtuhzs.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gymugygoa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/ghouqynwv.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gjbrwotpn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gifqadxhd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gxypftwuc.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gkhitfakl.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gyxotiehk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gaclnemde.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/guytjxhqy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gmkiyhasq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gqbullsaq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ggaiqwdqm.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzjlfgbqk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gjtwcxxil.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gcltjsxlu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gtibmhsof.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gkaasxlwc.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gwqekcfbw.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gvrirtwnm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gtveblgtg.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gxisunjwt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gaxsacjno.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gywgzrfng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gdzmuzssi.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gjpckvwdo.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gkmmkbbsx.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/grgumluel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gprbsycyt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gbyowjneq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gymsfigzu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gcarsemho.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gbxjboyeq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwbyzxjgi.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gspksokbw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gboncqwhk.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gncwqpzce.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gpdzftwyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gyanyagzq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gefgaruah.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gorluxavq.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gchyvivpj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gngfeghha.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gngztfcaz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gomfsohhi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gxtgpvcoz.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gfnynogtx.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ggfxhnuoa.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gycfeocht.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gaewwgath.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gbsivtqbw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/ggrlupsnd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gopkgqwub.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gzvxlibqz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ggzpagkfi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gcjbykdxx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gcmuggkrh.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsbhypawe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gvhwxbssy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gkpzmvdok.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gqjxrclgm.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/ghkcusrfs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guvnnxsvb.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gmmnqrnkw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gxokpdbch.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gecwvzjzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggthhgrrl.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/geeghnuqs.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gfkpijjow.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gpurrsfig.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gvvzmyocn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gamdrqnmq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gnefaalay.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gohcheqkj.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gsnzjftzy.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gfoipmffy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gsfaypapn.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gveizjedv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gskpjrbcr.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gjsqczyoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/ghjdrtdfb.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gakfppwda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/goqmrbltf.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gntmjynwd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gknxfshav.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnljgqkie.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gyjzrvzxe.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gzwngmxno.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gnvqtkcil.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gdxklqhex.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gykcyzwkz.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/glthrmwgm.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gxtbmheyx.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gdgyyyfzn.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/giqsfjrxq.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/ghadiabaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gekhbbkwj.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gpwhyttrm.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/guizvpxpw.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gnbhzvknx.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gerksoihz.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/glilnzscz.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gksshfnsv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gomdkbdtd.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gdylqugdl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gjaujbjdd.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gtzexjtfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gjhjnucbj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/guirebuem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gntwstlet.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gxyfpelzk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/goaoalqgf.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gdibuedrh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/givskhutz.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gsdklrrkw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/giyfjilsh.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/glqresgbn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gxkquiule.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gdusnvowm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gjqedjwjy.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/goeovoren.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gdnfalcyb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gujsvmqdf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gbooycgbe.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/giuelwwyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gvtqsjvah.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbzzdlwfr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gqdiepzit.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gvdhlemuz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gbptvrtth.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gwigugvgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gpyfsjqsg.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gqluxcwyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gcubyuikj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/ggjcllhkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gzrwautqj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvpygcyqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gxoeqxhrd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/glskxydkj.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gvqrbketj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gkuhrluny.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gorjityuu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gakowsdik.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmebwumjr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gptxczydz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/grlcgdcvo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/ggggermst.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gtngzcxiy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gfzblqoik.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/ggmcuplih.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gzajxdqhk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/goebgdyub.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gqqabqfpd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/grrvmvbbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gowhvhpld.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gfdnivvhe.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gyszytwpj.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gqoikqkmb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpqicrrma.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gwqiphryg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gqedvmbkf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcerhlomm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gvggogihr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gywlsyaaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gssgzoaeo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gauxwxadc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyzrsspvv.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gcznskcch.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvafujera.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/grlxbbebe.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gnjngvprt.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gbtimjtrr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gpomtukgc.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gtnlfsnkq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gxrbzlolv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gljozpijc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gpnnszjux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfjykimzq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grndbcjqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/ghcdvritd.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gghxelywy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gncsexbuv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gjgkwmkxr.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gxjejonwz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gsecdsfdj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gnqtgkncy.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gdwbvmjza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/givasdvnn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gvhujrcxy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gktgafngo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gnhkabeef.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gzvwurkqz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/geqrpnkep.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggoxbzhpy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gxrhelcta.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gadfzbmys.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdtkcxmtc.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtrsdaniz.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gnczksnms.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gmmvuwcwj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvkxzsoqs.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gdurfqumv.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/grhuzocmt.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/grwentvui.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gpadnsdtq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gwyvbghuv.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gyljsqkpa.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gzrdxpnmg.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gfqzeehvd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmwjjgvwi.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/garujfghu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/goexhafkd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/ghaekbqam.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggirrhzxh.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmvadmy.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gxkoroeds.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/ggqnzkizi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gqhyuaptl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gvpzbklea.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gkvnspern.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcvjfkuwb.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/glrezqkvv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ggpcpvejl.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gdlfcudiq.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/ghfjqpqkr.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gkepcqlsc.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gxldqwhug.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/glqhjgaqg.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gjmenffrq.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gxnxzrnvg.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gzxzqtetz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gmqujifsi.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gzrxojxzk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gnfyuhpte.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gdipkgeof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gghpvmphd.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/geknfdcey.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gpdsfgtxd.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gpmygtzsh.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gdzfyaqjl.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/glanugtok.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gnwkuwedj.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gsfcupoey.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gpkpmmwqo.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gimwqqbtn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gjstjgsyc.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glsjwohxo.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gratgboiy.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/glnjgstyw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gnieooqaq.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvmwchfyv.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gbysoofne.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gduqqqozr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/ggjwtgbsp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gpkfzxcvl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gyfacvrsc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gzxlexkba.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gqobjgccb.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/grmkltgaj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ghqrpmokt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/ghvffajly.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gefrspdzd.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gmkvlpfyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ggrlbpenu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcrfnubpg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gfjrxwjwl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gjtblrpeo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbhwnijuw.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gopdwdshe.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gmmghpnij.sHtML


<!-- 参考信息 -->