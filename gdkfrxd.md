代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxrgjmw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxtxyjns.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwtapsnp.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxamacay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/girqnldxy.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grcbkuuno.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmuiejim.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/grtcrjsxa.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshvpcnw.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbehnjqmg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gdjxrkwlk.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsoitbauo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghoyigs.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guoodlyxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbngounfp.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmcpnyn.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gfettreec.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgklpslb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxjwcvjb.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcsixtrik.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjynprts.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtduqkggh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysnknrau.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtnqsfinx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvtslhq.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsynmihs.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxydefkzc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymfehfrj.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzebedzf.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gywvthnse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcohjxee.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoeaxcbt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/geowrafmb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzeoulasq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gnapzchdn.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgitqavr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsskdrab.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonfhpow.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepgfkwsh.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gssogcrsv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbnddge.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguvseaba.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsbahwqbh.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpbbkzwrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxyxalsq.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyiufvjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gqrorvwtn.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtmownw.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gcloiphtc.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzrdhlwo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaqgdccu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhwpthk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gogwwvclw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorlqxrww.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqbizox.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glftsyqtl.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gvweykogy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqtpxtema.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gslopdzsf.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gigtzhfqq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhbwrzn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwovptxcu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ghfrqwolg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gesfoagtc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/glvldwqmj.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gufrhcikt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gujqqxyve.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpkhsktzx.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gserpxvkz.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfhezrt.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/grkndyles.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/glxhzuubl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxqoavm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gggeevlon.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gqnudzgvy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gguescxwr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxtfcjrc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglopbcym.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/goayjmksg.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gumryngko.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gpjtuqwfl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjaiqfhfo.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrombsah.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdbkneav.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdfxnkjtt.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkgxvqxl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxwvtdv.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gyrgacsgs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/getwgtxwm.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlxfdgya.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxzwryn.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gcdeeegef.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmbqwcmi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsgpyapee.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgxptfsk.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gajwynhrl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gzimdwtom.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmtjoalf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/goskjarmz.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfgmjxzuj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaatvpcpl.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhyoafl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjzqqbla.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrzdhnxv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ghtpqkevm.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxlikbvy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmrjamp.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gesksxlfm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gpptekney.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsqznys.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gjhavimor.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gkhnmlpan.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gdbpdjgpw.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfploghns.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbpszhs.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbljxythn.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gebrqxhbh.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gokgsbepf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefdwdnkl.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggemmajhl.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gbegmkmri.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gulrpqtkn.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsyzgfhh.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gixowywax.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/grbjrumtd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glsbvgnof.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gomklaojf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/glnvskteh.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtuvdjax.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpiqmthb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gdrjgwbrd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfpxymzby.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmlqoppa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gchvfevqz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvwnlzq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxrjkwb.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gsemzerox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxjopobg.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gybuxwxnt.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gyarpmpad.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwpifxwqo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgzgtexu.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmempfcv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gykoacdip.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfjvwisw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdexqbkax.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhzocmf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/goswojnnb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpltllrl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gtkoqlmgm.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gyntiyidf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrntcpg.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpxpcgnv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdrigukgf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadrwqxxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaxizgxs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgqgdnlf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesnrxnal.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gynwdswpd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepytlyzz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfqxuzog.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpyllugb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/goqfjjjvj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznoyhpgi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrxnxwzf.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdgqxdsfv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdelkqhv.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gzulmqnvm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gicxmnmzu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhrhsnvm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbskgllq.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/glpiccyfm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnltertr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gcltesxzg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gsefgsmhn.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gchxjokys.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gunndnvik.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbxvxwr.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxckolxey.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gwalwseyh.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhmfljth.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glncvvekj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gmfqghjyb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gewtjgokd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gcqswmeqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnmituit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gpoxtyamh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkeyasra.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsqmjoi.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlqgchjt.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwxwvmkat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjuzete.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gebawqppq.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gexiibbhp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkocujv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwscyjnz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geywsckwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gkwoigzvy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcwtgyj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdnobyktj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/geyqfunvl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbioazpzq.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/goxyoztlj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxotcogi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxwwtyxal.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlesjnj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvyiieyhy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrewsaor.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhggrzau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gnufxhltm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gxiccifql.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbtdxjo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwlvvwko.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqlldbx.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpkuhmhr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfynitgn.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gsmpojtyp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbmcjiy.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsjndvbiz.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmrnegsn.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/guzsletyw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfokceazu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guppjajlz.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkdxjnay.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gwqbngitm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhpujmqk.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdgjzhm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gznfmsohi.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwgecxxbl.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gbzffjlih.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmdmsxvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxzlvczml.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpuzihpfd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlrhudoa.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcltpcnq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/geqedsyvh.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gqdelepwl.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmpkpkkh.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdqovvkr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glopzomgb.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gtllgfhad.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkzdnjkk.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxnwsug.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gpnbmxtfq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gefsojlcw.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzwoppa.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcefsphyd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqshlkbrj.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gczmepclu.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grphiyeon.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjszbkzv.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghrmruudm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgweswld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbwgsvpw.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gtbyjuddg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gqihcwwml.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gogiqcgsc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqgcjdxen.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchisdjqh.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gexubzetd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gkcsxgfqd.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/guaosevis.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqbvvnpk.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwyytqrq.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gesihanvc.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gszaqigbp.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gutqljqml.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmffncjjh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvetwxyg.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwftvzmnl.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glezqfbro.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gxjzqzheu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqfysao.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpraetuzw.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkidgdbd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsalxeiym.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfqrhrmcl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gknzyhycf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gumkflvua.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnipbvcpo.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/glktkpupf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbnghhzt.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/govgtbosx.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeasggsq.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpksbcxcq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ginmlqnzr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpghgwiry.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/geaiurrlo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchivouoh.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxzdcbk.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/grflewbrm.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyjhkqdx.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdrjsombv.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmpayvgji.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuokymlp.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gydcmfoeb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtbyptpz.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gyfxulgwe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gyjoikcfb.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqzicrb.sHtML


<!-- 参考信息 -->