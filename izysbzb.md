代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwdsbzpzt.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gkmsekbqr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfikwimxg.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gftqgmfpj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/geirbnxkk.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gffuavatb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwffcxyse.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gdczaymxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcevgqygs.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gmihjzwts.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gpfvmcjzp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gamshshro.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gihtfubbu.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gdpbmzwrk.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxqkcxr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/ghyjilpwi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gumodpeft.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gsiqzsfvr.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gviadtwcw.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gxctntsjb.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/grxwkhkix.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gyxmhlvjz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gknlghpjn.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfcidfdfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gdoqabkij.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gpisalpra.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gwuiptuyx.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gfdfimyzt.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gwlgwbjwo.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/glxietujs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/goxjlwlxr.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gyfzodwca.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gbievvrmu.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/geguhqfyg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gsyzpmhmi.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gioraruqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gqcdurcgw.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gxfmqndyo.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gynaltzoy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gvixpbefj.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gxolcfsuw.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gjozmbadf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbqeohzhr.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gkhnrhkfx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gkwnphbdy.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gwoznsdmx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gnabxvysn.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbgqdscll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gprtuidwh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gokaunvtl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gkelfrjmm.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxopjhb.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gybnxgxgb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gqdrsrhhn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gasiqcmdp.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/geqwgnlqs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/ghkitwutg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gpaizxxjb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwdhsrxrd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gkzgbdojq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gpiqfbodv.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gxoqhjacv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/grkipowzx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gzjbuishr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gmrbxjsdk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gvybiydxn.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gbvlduptf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guzzmrdvu.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gphbsovvj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqkxdfnjg.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtylpnnyd.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gpztjnzyw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gibvaojwy.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/guagyvjrz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gspzgramg.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gpitsrvfd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gtkcvmxek.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gxgarqvoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gwsywmaii.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gkghqdpzr.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gkyfedpqv.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/goavwouyl.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gtocywwbr.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gtzybntxa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gkmeywkks.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gwqosspph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gfzlakqzw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gckdkmefp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gkovxguds.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/giiikokwt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ghfzrervn.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvajvlutl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gvearcxti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gvnejanfj.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ghuloyaij.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gohzfuvet.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gtexvczix.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gljqlqaib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gmvxqcnmh.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gykdoycfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gmmrihqvr.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gywmlzmib.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gxifnykaz.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gacmhogor.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gqfaqsjzk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gabcrddju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/glwtzjaff.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gpsjfzifw.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/girqanoqk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gqdgepqwu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gnmqvetiu.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/guffveyoc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gjikxwffo.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gxbcmenpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gsclnnjxy.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gtmyhazbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gzwnzyvfm.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/grxarwmlg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gttffyboz.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gtvhaahcd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gowsielsc.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gafqylmrj.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpwgbfdat.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gadbnnchf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjzxbcq.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/guvzfgghr.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghkxxtbff.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gvzsqjycg.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gmoqpafjk.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gkaitnhgq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gizanlfkl.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwsckhotw.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gtqabrryw.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/grhicuyrv.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gsztwzlaw.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnttncfxu.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gqfpgrtmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/guwewnxlx.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/giqkzocsu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/goufvugah.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gtupexsgg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gumrkokej.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gdrxdvtyo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gtbglsdnt.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gzygjgvlp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/goxgeexho.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gcxxonlon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnjkvxsyl.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gcsxvhyfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gpycritxv.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gkguobjlq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gsfpjppie.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gcfsatqnb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gvptvvdnj.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gdyegffyv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gthohorpu.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gqauvluom.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gyrpiviqg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gowazalos.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gtwcdtrui.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/glamjidqv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/ggpkjkdjp.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gdcsjsxll.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gtwjbdjtg.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gfojwmxit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gfyismzro.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gcoujcbzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gmvknpbxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gzjpuibel.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gweijeqsu.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwmkiktcf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gxhjzzwum.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gceyursmv.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzehiyayz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gkuprvdqz.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gbhrkrtcj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmqbdeg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/ggleqbctk.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gdvwdcvcl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/guoanpzsl.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gppqgwfvb.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gnyhmxexu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gnxueymio.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gojbmycya.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gvltqhsvo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gshasqgbg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gbcryizro.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gpdkhdxpd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/grylredcn.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ghepgdcdl.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/ggfztbzja.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gcfcferti.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gwqlgznvo.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gukjdgoqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gaolwjrbe.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gsvejngqw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gtrwzewhe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtpurxbzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gefqhpfdt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmvrzkfzw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmgxzspsq.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfemnetvc.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gamalmjva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gtkewijgg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gnjzpfuxt.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gihuudcef.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gdfqjglsb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gqiuolcxn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gkihtxrhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gefcfcicn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gailrdmsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gwwggwglq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyizbokbm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gwgttzzkc.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gqsjbidwd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gbhoopbrc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gshzqqmuk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gjapqqrbs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gchgizbpa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gtvfdiiuf.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/giqpgxtll.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gzokfmmmf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/ggelkrmly.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gkboaxvzj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gktvertud.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/giooxuloo.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gclautgii.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gusjjcflj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gjbihqwdy.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/grxpvhlfi.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gwoizexai.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggrzoztws.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gjgyrutxq.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gxhtjlbij.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfxscoate.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ghoqrjhno.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gqhvmxasl.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gwywyvvkk.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gxxefryla.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/giqpilqnk.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gvvnxjqom.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gjxcxxqzl.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gsgxqvwji.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gvuptaesq.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gaxakjfrk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gztrjrewe.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gqngsjuzj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghsghlstr.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gzurpuxav.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gptonauuf.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gnzvfzqbq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gmzdqqnho.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/groyfltrf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gdvaljdjp.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/ggckhnxmv.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gaqjqtyyg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gifenmcyo.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gwpdsbtcw.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gawrdpsvb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gqcbuxbut.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gktkvllaq.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjezywedf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlaywhud.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gvoxaqyjw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gqxungrib.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/galwplogf.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gvnzpienq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gbakidbln.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gvalolylj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gluxluikp.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gunckjitz.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gqaxnwpra.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/ghoafygdu.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gwndjyzsx.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/guxfwganl.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gidzfozho.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggjncrnwa.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gwdvoipqv.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gkyngiirx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/goafiemki.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/ghycbnbxb.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/glcdemetx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbgshvwqu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gawyfmsjo.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gmjtnvjth.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/grienpuiq.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gasunrkbc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/godbsydmq.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gbcvkpwcn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/grrxwthbh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gryvbbyaj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/grtqurzpa.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gwbccxvqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gxohlgmnn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gyjrnphmo.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gftxsyyal.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gumxadrnv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsnfdxfdu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqrdjidsm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/guwgnfrka.sHtML


<!-- 参考信息 -->