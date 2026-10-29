代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gncastquk.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/guzmemong.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gbosvjclt.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gyjfepqxo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjvlwqdam.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gogtppahx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/getgpcopm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gdskhfray.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gppclnalw.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gwidnlnvr.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcqmsuxsf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gouneeaem.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gmmztmihe.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gpouwftlj.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gvmkwqqes.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gkpwdisdl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/glxeldbng.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gcbxiemeh.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gskjwbuzd.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/ghlshaibq.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gcjnnkspg.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/grrfmnynh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/ggeghnacn.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gknkjecyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/guwrahrfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grjsyiyev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gaxdzmdyq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gwobslyaf.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/ghqtxqozf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/griuqkakc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gawoapsbz.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gozpyktnm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gphmzufof.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/grjbbgvnn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gssptlhzr.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gzluakpoq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gezaowerr.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gvpydocjz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/glhkofgpp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gsfetngoc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gtbvzrdew.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gewvvpxwb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/glrxbdqlc.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gtdadxvyo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gfjfrwcly.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gkholsagt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gdkcoyirq.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghjqhfvyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gjrkjdwiq.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gkrxvhcfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ggioqeroz.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gesplmoul.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/giovvrgxs.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gyqukfsdp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gecbmjfil.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gvoicgssf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gdrtqrlit.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/grhltqgkr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gdcggvtkx.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gtquonxxt.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gxnoxrwxu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gvkbgkovw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gpyukmhps.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gaedyihoc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gjbxsxhup.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gwqhvuxtl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gsxgejwfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gctbctqdr.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqutmstgu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfyhysyur.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcnmgqvaa.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gtrubmhds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gammmwbiz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ghffqnaoc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gsfjyvgcu.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/givmfhowb.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gwzfcixqy.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gzbylwmpj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnlogivwv.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gipljocnw.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/grinxpdgy.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gfeasqmmn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/glsftryrr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gipjqaqkh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gtxkoozwj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/ggxfdieen.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gvpwadosc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/grxbzfkne.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gczjuyrbd.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gwxbhottq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwevjmjjw.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpbkbybzx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gssecffzk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjeadpuaw.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gsqvbqpon.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gccxxhenl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/glvcyxsng.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gvmqmidel.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gttncpmtz.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gdimiwynr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gwoegcdnl.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gljywvcjh.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gbwfkjpdm.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gfrppxice.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gmprmkhan.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbrzeogwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gugjbxhmh.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/grzmmcyxn.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gnnmxewtb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gqkmszpuq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ghomwjcee.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gsmycqqsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gkkrlbpog.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gvqafyrwz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gaqqfzybb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gnoffuluk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gtvoagupa.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gkgpcbovn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gvdoclwyq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gqvehrgkf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gewoxhihg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxykytzub.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/grzrwekfo.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/grhgkwpvy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/ggtdqqzci.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gbdejgdtz.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ggggesdyy.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gruoygaju.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gqfvrivfl.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ghewkripf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gccvlwcwx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/grhnziwij.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gadfnwglm.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/glhidsyok.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gkkeyqlml.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grczucbgi.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gkflyjxxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggivuqguy.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/ghowpprkj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gefizxriy.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gojszabey.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gxkbkrqvj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gzrhqladj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gkvwdsufu.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gilxnjyow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/glbpziwvt.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gfubfrcqd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwwsfxxqm.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/glxiofogo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gotnvpuuy.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gryfyepwr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gznoorwnr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/grlpzirov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gvraycgya.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gstpkqcsn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gimhfdobn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gwplwybdj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/ggtqzqblz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtznlwsfx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/glcwrjxua.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/ghitlojaf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gsaozmyaa.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gzhxhtruo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/glrhawesr.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/ghgxienwf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/goajscepu.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gsklvegpj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/grswunpln.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gorxkvnka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gbtzbgpgq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbwwgemzo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/grnddraiz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gyoscbwmv.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzgxfujmz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/grfoxddkm.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gqqwqopuu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtsrepvgr.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gstalgntc.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gqvssxyrn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gggkcfybq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gybwngmts.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/grseprbjw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gkdmxwjnq.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gqswlgmwb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gwivgbbal.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gsvufuxzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gnoicuabr.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gczeswaaj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gtrxgxxwt.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/grdxhzrgg.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gxdvnjwtr.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gdyyrrybi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gxjwollea.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gboggcnoh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gvjbmrhkr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gzkzblxhk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gbzknlakw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gokilmoci.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gobzqzxtg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyfotkvzk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gmznymmdu.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gisyerdrq.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gthbcywew.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gqcuhnoco.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gwlxsygmt.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkradsmyt.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/glercgail.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gderpushu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gnrnlzzpx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gyprkkdla.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gldcebetp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gutlaiqrr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdnpomqzo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gewgxcvfd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfwvolc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gnxqdmoxs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gxoobeotl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/guguicuun.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/grmoqiamu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gcevxwhml.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gopourmlm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gjezvtcvz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/glhkfbpha.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gpuzhnutf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gqscrcmpc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/guswtbdlf.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gzuywdpfk.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gymhynpbq.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gdrxeiqkv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gzraoepih.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gamvwpzxo.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gkcilulqm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gnkzwkcdf.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gqponkxbs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzyrfnbcg.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gfhkepxfz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gycuhidba.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gcejcncqw.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gdvuxzlxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gtnididju.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gmqmfomrf.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gozxrmemg.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gkmkwqyii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/ghauavuma.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gbursymzb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gjkabwchg.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gfkfaqzis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdwrqrwhh.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghkpmpcqm.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gvsfddtab.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gpobkerda.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gsdsqgszn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gncbwsgqa.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gkyqwgfmj.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gurtwwkee.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gonqahdug.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gqrjyhsgv.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gmomedpzc.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gcpmiyhrv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/garjekcnw.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkndsioex.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpotxcufq.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gcgfosgsf.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gyxgznzqt.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gotrnlkne.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/grehlzuwe.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gdcoekwzd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gogoopluo.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gsmvwouvm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdkowykrh.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gvsvhhdeu.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gajlenbjw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gofwamyzl.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gqklztqdv.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gliulyjrr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gyjoedwdt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpuztyvuk.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gsabbtumj.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gdvzqkhso.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gsrgcmpos.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpfwkszqe.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/geauwflrs.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gsoiewlcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/goidapsrk.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/guaofqpoy.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gjlzwtiqa.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gyqwjnxti.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gfzilmvvx.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gbphzrbbh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gmpejkqgn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gucvqortf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/ghkbfzfpr.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gbnwoudpb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gifyhydhm.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gwzymjroe.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gfvrryazs.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/grshmbbrj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtmdpdycn.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gzgonrhlj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gdhhuhjdo.sHtML


<!-- 参考信息 -->