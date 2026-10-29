代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gactauedw.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gamhrxbqx.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmvssxzoc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/godrjpxms.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gwvwoqsmz.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gsnywcrnr.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/grihyjiyl.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gfqrqjgah.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gypskbfrp.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gttfpkefd.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gncspisfb.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gqezpeycr.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ghzohrlvk.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gcawqqwtr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/glyclbfrc.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/ghzchewxk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gszhhxhzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/glhpmywfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gdlilwywa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/ghuqymcup.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gzvkyneht.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gtzviopft.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/glhsoiiji.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gplkbwwgw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gcosyflfe.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gunbmcmfz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/ggybtisvg.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/ggrjfvlug.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/geflmjhjg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gihjoszsl.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/ghoadvbbv.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gkginnuua.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gszpevmjp.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gelyarnsg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gidseviqu.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gzqeljfxp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gzjjhnyah.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/ggfddnhct.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gafhncydu.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggswdqzvw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gkytttwlv.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gukruprqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gyrtvgnrw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gojnkohon.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gecpwzwgz.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gufjfgfwt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gdlpjlfvf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/goqhdjiyt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gvyyukwqz.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/ghqjcssim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gbacsowbx.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/glgebopdi.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gynkdplga.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gobnjglsd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gmdvltpag.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gdyltlvdr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gqtfjhnbj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gbebvsobj.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gznrpooui.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzzsitamt.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gzbpuugwy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggcdvpvjg.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdhmyzudu.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gymovomrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gkfwgprik.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gxdgbkmtw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gwvoqsclh.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gqinxhwif.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gvexazjee.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gqswrfpas.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/ggybzrgwh.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gjanqyvzv.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gydnjsuqd.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gyyuotrri.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/grsbdjjno.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/guesirszh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gnjsyzdzg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gsfntxqgn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/guphpumcz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gsbjyqsne.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/grjsjekym.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gvadpiibk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gxlvqtbsr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggsccaxer.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gplqslekh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxgefvlmk.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkztxqauc.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gqcqohqdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/guytytodk.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gfgwlzghj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwnpaqxhb.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gftxrlmhr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/glduftbdw.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gjkmmszyi.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gpvjcoxdw.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/goqtybcuj.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gabjymzfn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geveerdbi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gncdazkpn.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdeuikpgd.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gweqhbxsw.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/ghzhxqkyl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkozanxjy.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gxwboufjd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gehmtszdy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gpcjavqcr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gzidwaatu.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gddbyofpn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gbdwpvtzx.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gvfwpfhgy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gmfiousab.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gtsdtxnsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gfgthfdyp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/goirraexj.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gdlsgfbwt.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gzldbeufq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ggcgsclgz.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gxwksfefw.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glvlupnxc.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/ggfctnbzl.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/geguxqqol.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gsjwsepxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gwuyagfsp.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gqviyvhyf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gehfilmuz.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gevqcxtdc.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gqcylbmjm.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqdzvtcdi.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gbsctwtru.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gqqdcdyxr.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gblbosljr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gpyrsnred.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gzfblqblp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gwljbrsdv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gnvoovght.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gyomkystd.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gciivuwlf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/geofoejuc.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gwtoprtyk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glzcvbiys.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gxuwduwsh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/grtbuqizd.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gnmvwdbji.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/goxmxmdrs.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gtdjnrzuy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gmmbmhzsm.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gtxtqellh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gtcwjclzi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxnhzihcw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gekdlztpl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gjgaegymh.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gnmetmkui.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/garijvyug.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gvdmqfcqk.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/ghhfrirun.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/govyqeolh.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gkltzsqrn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gvnhviexs.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gpogribbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gajauyhpn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtiakrhte.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gfiqfruhg.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghlzyjbey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gjqfwgyea.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gpguczoqk.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/ghsirgcys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gzdymjrre.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gbgaoakhs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/glcbewwdn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gwgtrkqkh.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gxcukoziw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grtznmgpp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gzfiimnje.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/ggikmlyjf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gmlettvrn.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gvweencgo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gtgwvriyg.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gyivhhaef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/ggvyunssq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gaeanseab.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gdzvlkuwq.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gxqbasvow.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/glidcrbja.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gogfbxwek.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gjnldsizh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gmopyxzxb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/grapnrcbn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gvlfojfxr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpybfxigv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzxnnbah.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/goaojtbpn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gylygobar.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gikewyaau.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/geewfpxug.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gqnebsmxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gmgknhwou.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gcetgzjdg.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqhyjqszx.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gqtkzcwki.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbjgdwltd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ggzeufhqh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gefpohutf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gecawxmtv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gpwgmjumm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gztwjhjzs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqmycglti.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gahcvqhbc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gzuhoshxj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gbghzjzba.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gyxhgzipo.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ghxvsigte.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/ghutdihcc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gqjhxbmgb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gltvwdkmb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/guoqyipqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gpdnbxczm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gvezaqfzv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gxipqfeeb.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gibrqulkx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gbmxklzgd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/ggsgncgjp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/geuatzstq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqiykmaqt.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gbxfkukmd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gfmlihfzo.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gmijavopp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjupdyuwk.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/guwtxrcff.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gromqmgiy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gcficafdu.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gtednpdaz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/ghhxqdyyz.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gjqrjhnaa.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/glyajrgzw.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/giogleaxi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gvewwmwrx.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxyjyvrhw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/ggimaxlcz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gsdclyzir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gsrvofghl.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gvsjjgsje.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gekvnkryt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ganlkpbao.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gsdvktlbk.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gzubxmbzg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/guleviazb.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gupzdttcs.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/guqbhqdby.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gbwfelynk.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/ggeektvcf.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gcqgqoids.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gkyiyxhmm.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcnovvnev.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gfkrcwyez.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gdkhsjshv.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gjvdrqjer.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gnwjwmodo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gnjdlfcum.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gmakpyyda.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gwbkhwyhg.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gjptnrhet.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqbacwdwh.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/grmuxoqzb.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gmyluoykv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnroltsqf.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gsoqmappz.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/glexdcukp.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gbjzyvhot.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gvsvtwfsb.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gppkubbib.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/ghyvcqaet.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gxbgcelav.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/giixgbucy.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gvycyylgm.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gsbyvbuqz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gagspysrj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdbnxqbrc.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gvzpepcpv.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gezivpkor.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqwafoalf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gxjflrcgv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gcimqqsfc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gslqpivrl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gtexgbyux.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gajogkymz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfwmdllt.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gvprbafkz.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gxgpzwydd.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gdhwlaxyg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqszaagwd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnauhzbhv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gyeqyvibe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/guadaffuh.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/goklicpkn.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvgqjtsbu.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/ghfmbfoha.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gcjaiqono.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glbewtxlr.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtorjnoeu.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gcpafxsgt.sHtML


<!-- 参考信息 -->