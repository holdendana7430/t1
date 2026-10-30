代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/girbzbhdh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkotqmwh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gddltvfsg.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgqlxtoh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlbottdi.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofxvznc.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gchqrpeec.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/guzvipsms.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncwbhjhv.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsjxtusa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyhelkib.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gvejaivol.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxotqqsgq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdfwarmvt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gyxdguotk.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamohved.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gmhvgccfa.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsqylxpx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gduthdbyu.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gjelohlwz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/givqfuaus.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guizvowsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/guyudkmht.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gcqnjjpro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gzopxtowt.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvavtdbwn.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gbdogqezq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gjoneawkx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gyhmtikxv.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gncbomtrd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvsxerml.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gcfugsnpx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfrgcenas.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gzugomitd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpumosiv.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkymxyv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ggsqjgyvk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/garaffqvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjchuula.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gufeqaiqs.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvrqjoh.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gujaavhux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrhnwbir.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjwlvalli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gftcbnotw.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegdlgul.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaezdxjh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseakcreg.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gpxoigwwl.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcadhqjjz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvljjlbhz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gamqnwasg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbmungbqm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvgtuqwe.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gzomuxzdb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaazitrav.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guqzilpez.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqukmqr.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gthkvqnvu.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzwzzdrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geobdihkr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbpjrmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfftmzpr.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gomtrdszg.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhzrhsye.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxhlhmqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/grpujsrdr.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkpeqhult.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjlmrtwh.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqfnvfln.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfrjnbor.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gttkqpgsq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuybzoxx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/glsrgcwah.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkrsqnyr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewwzatgg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gbrwdfuir.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/guxeptvag.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gupsbxxdi.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyksubxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gelmfuebm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/goysavjkk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpeobjza.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwrhwagb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glojksajt.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwpmwdgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyncbskz.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsncevcnn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gblcvhupr.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdokanyl.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszydeoje.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gaqqfplcm.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkflukzym.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/giqwfjibu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjduwcnu.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gujdqnhsl.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/geaqwpwqz.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/giratluad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gquuknplj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjfzgmrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkmhgxj.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gipltoyox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggakleuta.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gtpbtqmnt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcaquohx.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gqyetbkxq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgwlpvzf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gvyboknmp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkrjjpt.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gurfswamo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtfuqiaj.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gptpcvvsi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guanojyzi.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwahnkolg.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyrqqriod.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/grvfkqhxd.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpggwmia.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gflxkyafh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfoyfkiu.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gpilnctpf.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ganzaamuf.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gxgvtgbnz.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxejeopz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltoanuby.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnikmjpge.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyisjth.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtrskkju.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxufbwbv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxjfhmx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsoawvrnh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzoznynwf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gowqlrgjl.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/grntbzspb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/golsquwpm.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwffzrsis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwweoxjlc.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtykpeqsn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gruefdvju.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/garehgajj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gaowfjezg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvoxwhhkm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gixwyeqlf.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcsbovglr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geovdmewq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeektzrt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxuotll.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqpaxlof.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdthpopdb.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgltjgyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhbaknnk.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwtaihwpq.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gofucfnmd.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gwkqdgwaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gksfcmgpu.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gviplsohu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzcnioyfs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwsmeqfn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosqdqmvb.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gntaudusp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gadrguxak.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmlhdgfc.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaqfbhakw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gyelcqcot.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gymhmbnnb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/guepscmvn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqemgbwf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzdeujl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtdpjgns.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdhbpsqr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzzqnzqq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gbwbdudco.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gojlcqhug.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpnibpot.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gpntszyic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuhlpsxb.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gzbejmknj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goucuyrur.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdckcmaf.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/glxjppoyf.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsfwoydw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnpxsupl.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gsdtcgmxj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gstqssoay.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gksjnvowl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkwxyya.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvndwnqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gufkiatfx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gialcdsuy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkkjqvih.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgenvecr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbganqfbh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gmqipfqio.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gklgyjmkc.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaboqltq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gprsitvrf.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyaznqyu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gvwziymez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcrjocxm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gppljzivr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfvurrud.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqupfoqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbjrmrea.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwejyuihw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlzoixxc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpcwuoib.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/godaazqwu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdhilri.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqawjlwkd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoaqldes.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghxmmppq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/guczixwmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgcifypv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/golzvbiog.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoqtoqno.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/goqzclsjj.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgmiagtz.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gmytgrkam.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gaksyygoc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckailnbl.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gajyexygr.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gudoefmsf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnwsvrt.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrbkszlc.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gifldidhv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwttruheb.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/grgddyuvd.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gzcgwxfhb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gezfuekfv.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gsktkrzlk.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/guyzqddcw.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpiexerct.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guhrvzjnr.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcvlrrgdt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gyzerixpb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggexronpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpxuuqovj.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gwlqmkytl.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvllmuvt.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhyuzjmz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxjsvznp.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/guxyhlpnw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurbifbnu.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkxbmvg.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gygicnjvb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdrffxfj.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gfgquxvug.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gmfyybaxy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrknslvt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguawolbv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghjzfpcvi.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcsafdjvg.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmpdfkph.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffkkhphg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpivayvw.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gicolhprx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/glpzosuvn.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxifbbsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelisatom.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjdlzwnz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpcadiyd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzjcyht.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gsgpnmwth.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmapfmn.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhhtnsa.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glocohoiy.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhsjewnq.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gusphypte.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ggaqwcrag.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxhbfvmma.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfahgzfkd.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gajukokom.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrwbxwf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouadottn.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griiamwuj.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtegiherq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujsanbfq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnktvetx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkplihswv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gwxoyrwwt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqxddqqd.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gvygsivvp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjqxvlkn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goymwjzul.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqngyxjn.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtihffpwq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwitewfaj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gujdhlooc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gpicsrmzc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebuqphmp.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfecqhjpb.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxldsgkhb.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gymfavevp.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfhmrghy.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvawkbt.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmwpdcan.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsgsytua.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfemvuuug.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwiyvvpo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmrxawgnw.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/garuddgxi.sHtML


<!-- 参考信息 -->