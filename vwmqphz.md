代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkcehtz.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gxwuleggl.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwggtzmct.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gfwybtwob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggtpaczsi.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdimvrvj.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gomrlwdqi.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gaerkiool.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gvucghiwn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyeotoks.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkxpmvvj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmabbtdk.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gbknekwbp.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghomkirmz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvklifecr.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gqsewlkgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gjrrefrgg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gytcxzvcq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsrdvpvk.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtayrghj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevfcovjk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkchqnqfs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gdzzmmlhy.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqcxoaza.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/glmvukwbz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsqznzyx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwooqute.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmehhnegf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjvravvl.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gienysvsm.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ggugxeudr.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrramem.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gozbpoplu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcisuobpk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpegaozkx.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggacgoehb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxfaqhx.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gspgyicgp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/guikwvskh.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/glkyqldpt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gpmfqyoom.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/grlrziiyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxbstfbu.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrhhgvn.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpvuzugqw.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvunulfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfrcsijyo.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbpyacwf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexzidaot.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgisjmp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueldhqjw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqjesoec.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcjzknas.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/govxfsxhl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guzfrejlc.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gtyahemjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtduigwc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfflajez.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/ghnnurtvm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyyswgfmj.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrbtepkj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gftenbtuk.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpajkdvor.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvzxedz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glthholll.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwytrpmr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwfhoytf.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjgwuvypz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxltovend.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gkoikkvfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcmtxri.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grdpiwwmy.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodrodoz.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grkoqkdye.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzazxzkf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfspvrjax.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxtasbe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbmskjkl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeezcara.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtcfiym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqwlipe.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gajpaberc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gqzidkrkk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gowkudgyb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gioyifcel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqdbfkah.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzdpxiu.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtmmjnxqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gxfslitrb.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gmjulzdvc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnrhbcx.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggemmtvkf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gfgmtnooa.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfidpwauf.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxiumbcko.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsodzdib.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvhmeziv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gugcybsfl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqvivix.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpyoenyuc.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqnebgza.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyyjgsur.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuxrilkj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gshqtubgw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ganabkgfv.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtkghhn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqprujijz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepcptwab.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxoojhsk.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrdjnwyx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/glqccpchh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdjboyda.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gispliidc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcslxsqb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grndzlczv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/glthygqir.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbqovwwq.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geahlpryr.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwzjiub.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqzndlspk.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gswyxuovj.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gruxqkctl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfspmrcu.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/ggpiosrbk.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gpyirecwd.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzrztrjd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gaacmmrln.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqxzzdta.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwliyjnmj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gangglxwz.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxerrguav.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsaneiuy.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gyidlqrfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwmaaugr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gkpfbwgnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyzxtthjk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybsrkqha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrfzdytg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxiinjph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsidugnwo.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gdefjkewn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/genwpkzpv.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwgytjqiu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/guvdtfybh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjouuryab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gmedtcfsr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxycxkh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnthjthe.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/girzahkoi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfopifxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goarxfcso.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gviorkkos.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gtcrkomik.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/glyttyaia.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/glprblttp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcbtgrnk.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvrrewak.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gcquzuxeb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaytwvihl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmshlskhq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkndglisu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjmirhgn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grpjlzork.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gkpzfdxvk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gixlvuyuv.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geppeawaa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyutmjjl.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjsufrcfu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvgpcvpx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfxznznm.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gevqjwaaw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcukuzxg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbdexxwv.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjxhpxy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gzchlbzkr.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/giselwhrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyoemtqf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxxmdwbh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoyxlrzp.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqeiiwhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbvqfss.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyyylglp.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokxpvqqr.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsunfisom.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqqbioiz.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxuhwbqhc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gablhfabm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqyesyg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/giewslncu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwgxllm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gdddhhksw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvuejfjc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxbwbfzn.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gernkwpmm.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjiomvien.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gfezsxxmq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gcddarrqm.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqumfaztq.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gzlofvsfl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfnqqpms.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gocvdypae.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvswzalb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfckastxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwypkjrz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/goeckecyk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqdpvzpt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/grjflkvkk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqeplhxs.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gajbkqqks.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gdxpupxbw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gemogvldt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/galsbttpv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkfzigsy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwxhhmy.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/givabshmt.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghfywonru.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbkisqubz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghxzpkvnl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgloidkw.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpsatwaoy.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gpexxsktb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/getntxzvm.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnnglqldk.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwrwbscv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgqhhbrh.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gerlherhm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewwqhsaz.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrybhdt.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxebkwhep.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gufnwxqui.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glcjhksim.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzuksxv.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqbwkaxi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcohismb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpdvmfpa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gcakezyye.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ginosjeuu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqjiayfu.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdudrzp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsjdktee.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gzptxghhs.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gslvpnygk.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gcocfjjev.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqcabns.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gejrmvnsz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjbdlcjyd.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwggunym.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfykzpjka.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlparafg.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpurirht.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gzalxbgqf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/giydppshe.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghmlsufoz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowfhkzj.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgilmmsi.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gvrlkylsu.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gtavaebmx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggwozmbs.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvwkycmo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gppqmgmbo.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gipdukidw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqojgckge.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzxnxytqo.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxsiasnq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gubtnodau.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guxfuxned.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxqcyoqb.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gsbhsozzo.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gacnjftom.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grufdzsie.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyinrgkm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/ghmqqorxr.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnjpxmea.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ghgmxxcgp.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzlpszhat.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzczehgpp.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzizwhedp.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtcckinh.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gstvbqswh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqfqtdjc.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkocywdn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtsiaunak.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gttepfysz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrfaojee.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gxbhdengh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkhadynx.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbqfhujee.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtredwgtk.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkeudwoax.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptyybgi.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzwxudfm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/grsfugtnd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqoeqwjz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisdgwygw.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmfsmcan.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gofoaqxmr.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyncwfrwr.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpxosblkr.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzvtintp.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gcnxdstqe.sHtML


<!-- 参考信息 -->