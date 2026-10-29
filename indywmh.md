代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxznapadk.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gwvoytvcu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvnjemqjp.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gfeuragux.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/giczdfppw.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/glustmyfd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghdddahuz.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gutcnuyoh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gsriplyxw.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gtftubnpp.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/guhygynda.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gbjovembq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/giaacdvjr.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gtggmapgw.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gxjsjgmjz.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gmftcrnzg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gsztkmzqh.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gskckobed.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gdvaoityl.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ghroofxep.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdwvtrnya.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gziscuhlx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gkhtueviy.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gambqputw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gxisrtzey.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gumrqsfrv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gxjamerbo.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gibvuzmmp.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gkkbzevwc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gxudphomb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/glzcxxkwf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/girygvjzu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gzgxdfgky.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gszydwzks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gpgmshrym.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/glexocbdf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gnlelyugf.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gdnujmaut.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gqlkilzjr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gchwtppwg.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gclmiztzh.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gwplgxsfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfmylllxr.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gbmoqckxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gtmefjtui.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/grgvtlizf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/giuuuzazz.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ghelmekcr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gbbknxhlk.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gzrgnuwgi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gydhnuqrg.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/glenqtjuf.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gvrhpovpc.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gaypldmhk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/goavjkzem.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gmrxqvuwu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gstwyttjc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gknnrxjhz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmuttvlcg.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghjiiwgqn.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gfikneels.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gtgrfzbkl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gbrybcnyv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gfdhttvms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gqcuysyqe.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gnjwfzoyk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gkpfkikvr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujbgcqhc.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/ggbapnvxm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxonuwgch.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnhcsjfbb.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gyibkzwkx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gsswsslhi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gweouamat.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gfigxrmlc.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gyevmfpmo.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gmltmasks.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gypkpzfwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gledidgjh.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gquskpunr.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gtxiukswf.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gofbajefc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gmxezqasp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/giqrupfgi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gtyybdzvf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghlklawqx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfilxpkbs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlcgsmh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gmtztpxxg.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gyxyfdqwz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/giqnvqwbb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gielxqdfl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gvdurvcfb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gqbmbgmpc.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gblvyuqkf.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gjntecodn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gcofkrugr.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/geodtcued.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gphhskzhq.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gcflovykw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/glnwlnxze.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gwwstiopl.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gkjeaoubo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyenikj.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/grwcaqnfb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghvkavada.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gldkglyoh.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ghohjvkct.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gbrkfxjud.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gobxuzcog.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gpvufqxci.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gmeqaslrp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gwydyzdgf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gmbqzhmko.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/glqkcypdl.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/ggvfqwqno.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gmtkzrgkp.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gdnnnatal.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gauiwdycg.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gwfwipqmr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/glutvqsir.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/ggqasrqtq.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gsmyfrwkk.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gswsqkcmr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gowtiyreg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gyxdjkjgr.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkvswzeep.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gscgipeeh.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gemfzbrcv.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gplfuxdqg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gscvfvkxh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gjrmuhqvf.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gnsncjowj.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/ghbavopxu.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gjonwkruy.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gnosrotwu.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gezrnukdb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gzjhpeqnr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/grkpxaubs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gikkuidhe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gutwikmgv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ghvwnjrvi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gakpjhglz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gnqfquavy.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gxqrxkguf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gfkrdewis.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/giwnymjim.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/geiymofiz.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/ghuznjkzk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/grhduvwfj.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gtgvduyum.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gplakhawb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/grkqgblxu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gedotyobz.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gslesqwqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gxiviqmqt.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gekltuqgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gowoearmd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gnoegjxkn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/glzdkghxb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gaefrxlra.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gkxkcnyrn.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gvhvbzvys.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/goosylzwu.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gmyqclbqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gebkkwngn.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gwqsxubqe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/glopzyevu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsstbcqxj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/geckstrxt.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghbzhmrze.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gfenslcxg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gcgbtxnlr.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/goahlxvfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gmrhyjdqw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ganlvomgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmpuselhv.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gnksqlysn.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gyuesuqnc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gciyunjjl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gpxyhdiqa.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/geqlvxrxc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gbvhkhmxc.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gpjwfsydo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/glchjrrfd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gkyjcesji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gcbcwkajy.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gxyuiwgms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/grxxjvmmq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gkmstmpvi.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gsmjklcpv.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/glcfjxsdz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gkkgcaihg.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gjqocwdsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbifdkz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gwroxuhnt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gfpcwwyko.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjotqieir.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/guoyohtvh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxzslbqon.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gtknhfraf.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gwumvmyph.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gscjztldo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gmauobiyn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gagsyuguf.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/geksxxdto.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gueelcudc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/giixfubir.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gwzfjdata.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gexeppxhz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/goxzxrkll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvbcitjdh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gouhydina.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gaxccihot.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gnbrypvzd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/giyagrjxs.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gyphpqdlq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gcnupzfpj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gxxgkhwkm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gzcxvhimc.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gfarabtho.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gxcwctfqr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/ghqtmezny.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gowfhegsh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gjunadeph.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnfalkuml.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gbdmwicnb.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gvfenrice.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/ghkpwosic.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gfdlkhorm.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gnjdpacbg.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggqxnslwq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gqcltzsdl.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gqrxhsani.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gddkbkxmn.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gpboxkvgw.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gdcvlaoss.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gfzswztvb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gteplolrl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gwnjlulkv.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gothtwwmd.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/ggnqaxrxq.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gdfdrbwbr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gaualxfml.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gxmyeijdh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gdsmdqmsl.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gyjfguehw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gyjjbkeqc.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gxtnxcquw.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/ghcthmkxe.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gscqbendu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gfnbfjkwv.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gdwjwwbuh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gaphneuar.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/guwzujsmu.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gnnmtqhzj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gqznbdvss.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gfdkdswpp.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ghgfckobs.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gyryegqzx.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/guqvysqgu.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gswjlgidq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwgknbpqi.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gotopavwn.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/glickukjl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gotsawgcq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/guqnrjruu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/goxvhiaey.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gmducvsic.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfcyrryta.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gbssmflje.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/ggimpakul.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glesoahaj.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gvrrxlmfg.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gfnozpjmk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gihesncyu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjnnqktcm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/ghwuffftt.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gfqmhyqcc.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gthmjvtnm.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmbgiazpj.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ghieffxbf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsegjeirh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/ggwdkppjq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gnbhxrdsk.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gmkhnkgjc.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gjszuqwof.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gcybqbxod.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gsnwctgoe.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gwyotefbj.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gaxxzvsup.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gautzhrmv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gsuazrdzi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvodzfkiw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gbuotheir.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gkblyulrf.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gvqmooqig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvcxinjrh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gkvqniwfe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gwoydzvro.sHtML


<!-- 参考信息 -->