代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gswbbbqfl.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiapgcye.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gczdsllrj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gefuatgox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gjspsfmzg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrzdtee.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgtqxnt.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijvaxdhk.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsglshbt.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkctgcii.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwclrjtpc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujrjpctu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/geknkelic.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhqrojah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gixpzeryj.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/goimqhfsa.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gjxlhhlpy.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnrsphnwz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gjadmjxgc.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gviyarznd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzfzzbqi.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvigvxfiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrryrfk.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvamhgwvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gaboquhnp.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gklxyqxmo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxefdhuv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmxfkrwq.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gezjoaaxw.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/givthfdoa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grvdcraun.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmyckizj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqmulshx.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/glgpbuwlz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gtxlalyfy.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnebkwyn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzokcqfr.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gjkbyqbal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gochbtkuf.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqjvziuaz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gcbktlsdt.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuivwecx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnlafbc.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoraestj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gefsqtxzv.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxrorqsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gefsfgfqn.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/grpsachnc.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gqlyngwky.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkudgsfoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gykouyhbw.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/giqgcyyfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghivursso.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctbxtzwg.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gwhygutqg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfsmgneyj.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gooegquqw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyvbdiws.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiazttpi.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gkxolverd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyzbfvmpq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gaokniqsv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzaczwaf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuorjfpp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezjngup.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbzrfjmno.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gemzeqhcj.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjwqjcjxl.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmtwfkcd.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcdjgpbs.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnzbykb.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxmcpxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ggdldemim.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gminoxzjg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gczlmrspa.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbtbpgda.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxzlkczzd.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gmoyaevrx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgvncjdb.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gprpdrmxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsurtryx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntpuwfln.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gprgqgitr.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjbgmbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gralngibs.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyiiaxsg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gxjlvizjm.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnikomxcb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjppulhe.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guwbihkue.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzpgcqdu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjcpucz.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gohrofkxc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqcxzzxhd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrczwdyy.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdesgzllk.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gydtoqyyx.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grhewsigf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guygspwtn.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjaocyx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuomsish.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/govovkrbh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmssdphdj.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gliuqgyyv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gpakvwjcf.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gewqcuqgn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gzecjfsnc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkyusax.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvzorrw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcziivio.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodtfkye.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gcovejfch.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gkgbeqbyq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqovummyj.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdabweant.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcbpnppbq.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstrmnhc.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoustilp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngonkwha.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gyvmfllas.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/giimddrzh.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyydugxx.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gxwjpqcve.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gncwkmmcj.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gmcnlqfan.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjyzaoxt.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjrnactpv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmxsuxcu.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/genihmfct.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjbskvhp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdmflshe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrjtrss.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavhokalw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdrimhjs.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gwcaamasc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwisjvvhr.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/goslhsbez.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhbrliew.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjgplyzmw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/grwbbxjcy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gocfqkyys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gpalnsyeb.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiuodkqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdpjnmvr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgwcctl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfkfjtnr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geatnsrwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwgjijt.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaocesxb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/godmgqmjn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guovsmvyq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gddoualjg.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gzgklatgm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gelijgtgh.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gekwhajms.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghehlyzyw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwktwsrlc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gerrnlynr.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwvqfsemc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqudiatst.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwgesxwde.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrylvff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/guepudnjz.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/glrwporah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwconwldn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcfguino.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gswknbtrg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmssonkld.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehoerwin.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/glcofwhhs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffjczpxl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapuwtweo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/groeogitc.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gzrocvdcf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gweyxrfsn.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomycwhil.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ginpbgjdy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylzwhpf.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaipqfsfs.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gnjjvixit.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/guavjwnye.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfvrstve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuyrnkhr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoxisobc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsrsmsns.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gztjoquzj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeofdeub.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzalaojbv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbuujhdl.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjqzyzerh.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqcfmijzh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabrjixs.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfrjvhn.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyicnrqlt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmteopoak.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gmuayjftu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlllckfg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/giztlygnh.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipaogyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpxtgxem.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnvlakopw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoxjmiyw.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvkfkfcn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gisnyduza.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwphgcxad.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gikpseagb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqarnhl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpemyheq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkguykak.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gojdzwepn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gzolaeghm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwooxabxe.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxmflkc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrmzivha.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvuiliop.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjwqbdej.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlzyafik.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwguisrzx.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnawjwzoq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkovysykp.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/geektutfk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgavcwgf.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdwjhdphi.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtykavmtd.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gppjumnfy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzounzpzp.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpzseattm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdmxxehl.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmrfvor.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuvqnnqg.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gblrrbwpa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzfygqnrs.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhddqek.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/grbocnzgv.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gpmdkfvoj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkcqddgmg.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiefmigt.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagxmlscb.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhijrztn.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gyhtoqumt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqywpeoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjarovza.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gavtchtua.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljbkejy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gueaghrzi.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gnxzazzqr.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gobpfbkws.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gwjaotegg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpceylwi.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxlxaqft.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggygjfefp.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gskguxkua.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebayvhwu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucdpzjes.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gplejuyxe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gmndljaii.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicjphcxc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyyvwwyff.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdmebrzx.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/glhnzoplf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/grmrizqjs.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmuuowzy.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grutppbfe.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymdihabp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gudwwynvp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvoyjwfw.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmapjbyl.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/goyymvopn.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdlwqokuz.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvserutn.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gklltnegc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gevnfefnd.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqcphmnu.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gekbvqvpi.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqyorwjdq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxhxfzng.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzvzcvxa.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvlwdvc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gavyclfdd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gucoyiugo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnkpgvzd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsefsgrt.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/glqtzhmdc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/glpgxdhfo.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcufmghn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glhogfnls.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcsastwu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhctpms.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggywhdsub.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/genbklekp.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/guurvahgy.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzotecdr.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/guapqhrrc.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvdwlmobz.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbsqhyui.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gclnoglvw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzufulpx.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfaclgqzr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagjgwex.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooxvieiu.sHtML


<!-- 参考信息 -->