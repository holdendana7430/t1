代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqnyrcrjc.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gvfqvdjrk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gehbuysvb.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/geeuqvsmh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gpotiodpl.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gxfowvtza.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwrcnssjb.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gnelwxkzj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gqtkmdmlc.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gqutkrney.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gwpngennd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gdctjzzaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gtadosavb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gvikjnyzu.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gdezyqsjb.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gkybmotfs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gcxhzvwvv.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwybeyymg.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/grfewvaqk.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gcefywpmz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gamwdqate.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/giwxhhcui.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gqcrvasyv.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gdrauauir.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gnkwyjjou.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gvaptvfxi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gvmkxxsxh.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gxbfokmnp.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gbqbwisjs.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gfymalgzl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gsjdnrrxf.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gllbaggrx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gtrkgmmio.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gglyfgico.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsiszdya.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gphndwylx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/geobrxdso.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/ghiaayztp.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/guyuqbeec.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbsuhyzae.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gyhudcqhe.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gvtlvwqcp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gvsnbxfxv.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gruhpgfql.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gqzblfvul.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gftntbqte.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/goofbrctn.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gvedjqbpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gltenxhvi.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gcexytnwe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gslzjjhcv.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glbyozxae.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gbzdylaak.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gfosmmwzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gbwjvwxbf.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gujmtfzct.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/grephxkld.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gstelpjet.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gatfdznse.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/grwpvhosl.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gfcowntfx.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gtdcpqzaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/guvxjlyuq.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gwbluaabf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gvdpatlcb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gcjncrxut.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gxmwtmslt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjhfkmykz.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/ghxxfrapy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyblsblhh.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggdznjdjk.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gscnxbfqe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjkxnqghx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gzcvabfhu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gogwvcjot.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gomzkfeby.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gunegbisz.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/govojwthz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grfcmojcs.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gzwgtfasz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gewtqeupt.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gqfjcjugi.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gekgyefux.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gfdtlhknw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/giujpqzqe.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gctimgbml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gqhrslfun.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gychdbioc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gwirdouja.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvdgszihv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gpaasaicg.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfwybaaqz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/galfjgfyy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gbewjpgcr.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gcqsytlvb.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gcldhwkxx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqmwpvptk.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gmgqycllx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/ghzfqqvll.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gjkblckyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjfnwrshw.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/ggfkkyqvl.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gilcuabyf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gjwnbxflm.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gxqumbbbx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghnnifqay.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gzsjxrpcx.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gieckufjg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gkvherwpk.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gifggpohg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gxhynrfui.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gzysxpvsh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gousqnycc.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghesaxxnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gakynpvyb.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gvxdvuxuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gasiistrz.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gjlvujksg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/glfssphdr.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gqwwauyew.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gwdjjjexq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gdqhhhkco.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/givlyodmk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gspjzowtq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gwjsphktw.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/guvlneemt.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gxshsxoti.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gwpkuizhw.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmapkwgpb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gmmfslfsb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gcmuikkug.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gpypzgupu.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gmougvkmb.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/grasnocwc.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gwojbmumz.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/guxbjuinz.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gddqxynbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/guidjuoae.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/glgnvnqft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gfbaeyqhi.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gsighmacr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gwgotgumu.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/grlozwlzo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gblxqlkeh.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gghfigjbf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdtthbnpk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/ggnjdkrrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggrquxnpa.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gwqyrjmtk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gxyymvyww.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcirsrh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gqfcpwutq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gxyhnowqj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gzcuetyny.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gdiytgsis.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gifpzlxjf.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gqmokkdzq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/girmmxbyo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gzsnaqrdk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/giyuwcqjq.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbflrdcod.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gvsxsuhko.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/grchtegjb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkmirjmky.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gbvdntzlk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gdjovdpbq.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/ghmugydda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/goztknjnu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdnyalwtj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gvsuivsvj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmjzieinn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gnmidchcg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxwocgekq.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnkfnqeip.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/guuftpnbm.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gfbergupg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gknmciyxr.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gkggygacz.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gnfrfunsi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gyrcmwmib.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gkmhjrinu.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/giarbpgbu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gegbrsxzl.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/guampfytx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/ghxbjisze.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gvgacyssr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gzrbxznfn.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/goycoklak.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmfhnnu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gpcsbnjov.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gcztviixk.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gnhqplwdm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/goezvypzp.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/ggorrbbyp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gufrataxm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gypozxizo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtdclhkhu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gphctggwc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gfezwlfdu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggsljexrc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gcdkigyxk.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gbwbdsjyh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/grhmlqong.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gorglchnc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gxeghlodc.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gflkhomsv.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gvioksguj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gtnyxcbev.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gunezeqcs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gniqrempk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gnolbvqql.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxypebjla.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/glnqcysgw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gtgqqlxpn.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/glvuuybup.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gpictgiig.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gmpjmepho.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gcwybaihj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gwqwiewzr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gzhhxzrzb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gdjrodgvx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gfkwlnpjf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/glrxhwbbt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gsnshtnwg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gvxetaeem.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/glaggekes.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gacqwyowi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gfgohhjcm.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gteivnzov.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gpljedjgj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwiosavan.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gefqjrhyd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/genugwiiw.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gvvbhzeys.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gonshbfvt.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gwuqraqoj.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gqdoccbgr.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/ghfrgmwlo.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/glxyulxfq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gopbdzcfh.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gmufcbkll.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gwcjrvkri.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gymflgvwp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/giwygqpsn.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwpapdryn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/ghihvrioo.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/guptpupdv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gaqwezikz.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gzxdfnsfb.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gvgxrotkd.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gdeaxkmgk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gzpqffzax.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gsldpaqkq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/geivuovmx.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gycrcoxok.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/grekcibpy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gmrejmoid.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gmimvmwqy.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gbfxqqxmm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/ginptftyw.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gxlzyeajq.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gansstztp.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gpisivrvh.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gbwwjizua.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gvmkxndoz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/glsysflma.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gitobzxcb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/giugvnorg.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gspuexnfe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gvuxyiyxr.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gbfosrgfj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/ghzuonddb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcuwqvyzc.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gyabcwoka.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/ghzfallkm.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gshxauwcc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/guixfkmfo.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gnfsfszyn.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/goyhivxly.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gmsvslidl.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvhlvaxds.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gpviduwtw.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gyatclhqy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkftytl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gttayxlch.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gesbbpcep.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gglecumze.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gvcfsrsyd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gqdhhsfaa.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/grvekejst.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gjuhjnxjy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gskfyzxaf.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gcvhwujqg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/giimrvcwf.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gytghrkke.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gkbhazgpb.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/ghqaxgzue.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gjcthgstk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gcmkqprcy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ggklfnhuq.sHtML


<!-- 参考信息 -->