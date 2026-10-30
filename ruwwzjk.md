代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/glhtzlmsz.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/ghmjyurmc.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfbifkxul.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gptbyotrw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/geynyrybt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnepixlzs.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxiyflik.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gznvmlreh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqyywsfl.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/giqehwhdz.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/ghcwezlit.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/glplrwlwm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzcdiyss.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuowbioz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gcizieald.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxrxipiei.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gecisodae.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/grkpbznql.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/geicrvehq.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmzqnitc.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizzjnmli.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvnsfoyme.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpzsajv.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfvferzgv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gmsbuwkct.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gadaoouhd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gswtemtwv.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/giquamqbl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gstxbpqlo.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsqkkmqu.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmxjdqnna.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpqukdpl.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gkosodylt.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnusdktwz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbhcbijry.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghllsmokj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhbzfhco.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gkphjzhhz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzguggfzs.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgnuowqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnzaacgr.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/grvfqvrow.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghjyrzgov.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqysdtxs.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegnotus.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gyozlyijl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpqlvteyf.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtqghphd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gikbmjrqw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaycxusav.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzcwzwgt.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gxymjerjr.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjatlig.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/giucruotj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzvecvxxt.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/glbifqqto.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/glugogxql.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/guvfmdfmf.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsxlqlpn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghbwxegkr.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmzrvvgqs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gstkugdxt.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrafvmmp.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoajijvi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giklfhmfj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guqvnzjld.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkodgotu.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gmfrhjozy.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gmqlcdjvb.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gaufcvooa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/goynnqymo.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfvmiuzct.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdcsqorc.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gndbbffvq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoznnovj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwnaytpr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmmxwgkm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjftjdhr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gmarrppxc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gunzlfgvb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gqnwlcdmd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfupenara.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurlqhhxw.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtgljyoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ghpbtxuxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmkngjuy.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdtkpoiq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guvdiljed.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmbaficj.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfecknzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/geshkhmgf.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gchmlxtlz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfaxlkan.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gesulhikt.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/goyztmmkr.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/grrqodxql.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuyzqrfo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gosmdpouk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganyhcesb.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxajceisv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsgcrhny.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqrblndc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpegiiktr.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbczjifed.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/glzlwtshh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtkputkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvascisc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzldoedug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqlyzdet.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gxeqsbpqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gzrsffizu.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gcmhwkcnn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gswdoxdik.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxtphpuw.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gtxlutupo.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaxgxwmu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlxqiryy.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/geedgmrlq.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/geuntzegh.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhutrcbi.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnsxjhrp.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxpvhbga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqvkmsc.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyeqbzvy.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzbqaoed.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gpijtsuok.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdrwckjs.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gklfzgcia.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gdetyejwg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmenekxkx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqeopyhz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqgnsnw.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcdvrcqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtajdehr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrpecptj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grejytgwc.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavwvais.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjmtdyhl.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvlzizpb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwutijpme.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gdlcfkpid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmvrkobv.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/grypyzjgt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpqzwwov.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcppljutw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gyudtbzrp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatirnamr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpglbyia.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlztjucm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbglqtry.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzhvjgflu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gpqlerhim.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvcipkyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwchvdxh.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gpcdytlzy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfmathnzr.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gastbwxjg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/giabuodjc.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gytwutvnh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnwwckon.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gedabloih.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhvwtpah.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxcktkp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkswnzofm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbympsags.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdjzyen.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gkwgorihi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymfyljvu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gytnbfkkg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/girneatam.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/givaalbqb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gtquuytjm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggdcukifr.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gxldhojzy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxmcycrz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuiunhim.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtcizqsc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbgtkaed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdltmjgm.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghtkmwnry.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfswftcv.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnblgmymv.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/govvlbfrn.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbflhluu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcitevysg.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gplqoqzac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gxqkngsrn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gpfvragur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhygejq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhjuywrz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gfzisnvpz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvyduwsk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpbydjek.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gptdwgpul.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpinhdbyq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbdnlmp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvihztmxx.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/grsdhlnkf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzsoqjim.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/growvpnti.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkkvztdza.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gijuunmlc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gzguwjpzu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gndpyxnjs.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwavlvbx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gldqakoeq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbvyoipr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowyndpmy.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwtmiaswj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gwlczvauo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzqlxhdr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpmqikajb.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/grxjkpvdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gbbnuuutw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtisccduc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfvzqod.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqrttfj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmgrgdcd.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyqdqrsxr.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxfgoygq.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gohxevcwe.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/guegaipww.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkkviorg.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyloihqeu.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gmaptnost.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapbuofsm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbropetoi.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/glostrdji.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwkeluyc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwjlyums.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gptqhinrs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgadvuiv.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gappifcvx.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gwnetvzeo.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxvdqcyo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrbzeuz.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goqsuvcxk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcmfxirq.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gliuqyiqh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjzrnypv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmifijxb.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbyqxvke.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyevtwqoz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzevtxbpc.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gprfqluei.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdpomwquj.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gceiqqskr.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvghhmgv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/guheftbtr.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzxdxygvt.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gquoqfzpt.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpvktago.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gddrrknjv.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gshodduzu.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwmddfdad.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvyysgvc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnitnnrn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gmhmdrlsa.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlulhqju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gsvtnoemn.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gybjlrnkc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdynwanyw.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqxtvwi.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gycprspvs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/ghuxyvndd.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlrbpnai.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gekntlvxk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhtbhtl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftokulp.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqnswzl.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/ghxkpbayo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnkizbmm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflaqhjyr.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gnbvulhwq.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gsvwwbdee.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gxxtlxvqz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcwdpqdu.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqcsvkzi.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gifvaaqbu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnmxproh.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gazmqzzoh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcemnmkp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtebwjsyl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhixlyv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnncguqlo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpgjrbtv.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjrptahjp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gghphdcra.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkzmderbu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdbycexs.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsynvzcpt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gwwoiqbaf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgaowft.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpzlmvmy.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzheetvrs.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gehfetbri.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gubtmpnme.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gvhbtvplx.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfdntswi.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gqqwpqeul.sHtML


<!-- 参考信息 -->