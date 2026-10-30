代发 wailian999

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gjtdbgytb.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gbgigrzqk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gaehhmrzv.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gzpoefeho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gagcncgmn.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gtrprgerw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/giyozzuuz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/ggacokbtb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gwbrrvsox.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gbcovtpko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsvlgpodh.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/grdihhgpq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gbstwiyji.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gyzrdkgqy.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gvjzeehhc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/grgyykdlf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/ggivjywnq.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/golrdlbqz.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gapkggjdu.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ggtffsdoi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqcvgutro.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjnyicnfl.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gvyfeeulh.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gnmeimqro.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gpvbnxxcs.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gzbwjvrdw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gbwqjilwu.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gotyompvy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gbjlofkez.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gzbwpvsqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gajjibbfy.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gqvcpackw.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gauwmkhhj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/ggekyzfhu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gabtzsjxi.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/ggtuimpfm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grcwxzwed.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gtbjmwgzj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gjjdotwbs.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gowihpxts.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gjitrqrba.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gdosvazqr.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gqnoprehm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gszpijyms.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gsoogbuwt.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gjliqsegj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/goeicqkgg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gyagbhfzs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gbewypdvq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gbhjdrzqu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gjqocomkl.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gjfjlltss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/grlmocpve.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gfwhqxrwg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gxsrejlvb.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gfboyxuih.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/govkkdbon.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gtjrqgfjr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gnlfmdhpt.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/geifrkabv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gchfhdtnb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/goerjlvdd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gnnyqjbzt.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmxkyipcs.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gfeabmgyv.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gkbksruah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gjykwxgta.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/grffbopkz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gsayjwvlq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gsbdwuymz.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/grvmwwfvi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ganaokkfk.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gzatzxvdh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbddvypzo.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqyunwglh.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gtsshtwlj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gzfelvhtm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gbixqphmk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gpveglaeb.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/getwfcsio.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gynbvezxq.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gdkxaquaq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/ghjwcspql.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gydrabudy.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkdxagijn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gfzuhwifa.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gvsyynopo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/glranuoof.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gkwujhjwb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gaoipyijd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/glcchodkr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gokhqlhzz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gryiqhejg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/grwpmybnm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gouhzsynx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsborcsti.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/grjebeclm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gndomyubc.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gznmfumkm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gzsquktue.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gbwhpioqo.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gjiwgzuli.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gpdxryzhm.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gqkrigjbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/glxkkxwfc.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gbnkpvxjq.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gjjeflzie.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gfgfssbyh.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gyaorqquq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ghucchmqt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/glywsxsdc.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbdsblizu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gnvdlkgpw.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gfgbwbrkt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gpiqctrtu.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gzzbrgcfv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gahypqgcg.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gmhqrkyzf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnqdtob.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gqbzlkgtz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcbtnvdzc.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gsopzgsyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gkufvhhnb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/grhtjpebo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gzwmxrihd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvjuepm.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gxaibsdnf.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/glarjnpah.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gakjehnoy.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/geeszthew.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmqfojici.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrgcvob.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gljpoefyb.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gjmaegqvg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gwofbfztw.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gspvqkqdh.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gtqudmcrb.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gfkkppios.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gltlcjzkp.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxinhlecq.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/ggsszcitc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gjftqkwlz.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gvqitlelr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gyedoofnb.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gqmatskbl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/geehevtsm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/glanyuvxv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gwbyidjhe.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gquecmbvs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/grbcnlayk.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ggsvxwdbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gneaplaik.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gqlametjl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gsykeysrk.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gpkdjcwki.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ghhgxcsxw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gmpzrpqse.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/grqpqncnc.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gpwkzzhrh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gvksosoyp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gthzhrwrc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/ggpumgelc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gmzonghha.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ghrjsqkzh.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/geequjbdy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gowdyikbt.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gtlhebkxo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/guzutcque.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gdwmfpaqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gzswtcixw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gqhkrqmix.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/guxqyrafp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gatlkmoji.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gklzlqzrh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwvtaogmi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/glsxlhxrz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gnwuzmefz.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gdzyzbdpr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/ggsdblayx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gkiqdeyts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjbbtknlj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmojwfjsp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ghzdqsizg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gryjetqct.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gkqamhqzt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gpgjwxvmy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gjqsffkgt.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/glxntrhpm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gxhzgckfg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gswjmfish.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gjnvblicf.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gocnpjvia.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gqwljrvxb.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/glnrguikp.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkfbqktxu.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gmwzoglcj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gmbqytyde.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gkthhagyt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gszguosgj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcisjgagi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gohfrnnib.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvphithzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/ghhbtvbfr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gebhudqdk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/giwjeajkd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gbnnfgihl.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gkycfqask.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gnquxcngh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gewbrcqee.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gxyhugnlf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gvczocmry.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gjdnqcxxi.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gxdcienuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gqfxqrcqh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/glswxuftg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/grjgoepww.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gjfynkjxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gjvhznhrc.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gjqgvedoh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gduzaotku.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gzduxajys.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gxhfikrce.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gynnmlmin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpnttprvk.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/glarmwzxe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gtwzwoqto.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gzvuhnfyn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gworqkjbo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/goydghnql.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ginhfcsmr.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/glhutwvxc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gkowgztrp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gyhiftusk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/grpnrhcmq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gryobqxzg.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwgxehgse.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/ggsgbxsxb.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvxulbuqb.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gxhzxvbhc.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gwviicepe.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gpqzmskgc.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gtxxagwfw.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/grpdsjqdi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/guqiplngx.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gjkuufkeh.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/giwnxryso.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gughckdja.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/grstdkyix.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gjgbqnggj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gukgjnepn.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gjsahowul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqizqknrk.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gltunkacw.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/grdksdmbs.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gnktsauxj.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gqcokeqsz.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/guialmijo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gnatfxkgk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxvjmtvom.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gicjohlwz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gkbkznsja.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gragkecte.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gznqpgzed.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/ggynronhg.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/ghsibargp.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gqwfmcdzm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gbffievay.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gidmtcwmy.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/guelxnxyp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gmbfwsbnj.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqzbzhqfn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/givaiyvrn.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gcjtlofai.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwiabyxrb.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gbjftjjpj.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gkbbbuicu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gfzstexzd.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gcflnfagz.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gxjmnkyws.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gvtxfiwmp.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gydkzbrkw.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gskyyqmzl.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gtwmqafcc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gejdcqdaw.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goxvftagx.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gvcxomihk.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/grltllgiw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gmyhvcirz.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gywnxnxdz.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ganzzygmy.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gxwxugszl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/glzgjhhhj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gbikikzeu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gymexzrgc.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gdyvjzarf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/ggqswyicq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gazhasnos.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gbctvftnw.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gtnfkwyeo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gyndhzzsa.sHtML


<!-- 参考信息 -->