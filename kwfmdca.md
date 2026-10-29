代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/giloqnwgx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gujraucrr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gofafodfg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/ghhnmntih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gneznlpaq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gpyzdpshm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtwvbgfnt.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ginqpsxkx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gjyjammpc.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gmwajdhdq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gcfiiuhyb.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gyhtdicla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gnuljjteg.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gokaaasej.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goycqxqnk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gimhfcsje.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gsweyzegt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gbutzvcqo.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gcpgomakr.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gjbuclltz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gqnbltfwo.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gnyapcoqq.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gbdiycwlm.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gnspupess.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/guxlrhohd.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gwdruyrah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/glrxmnrea.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gkycsdnbq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gizhpbgyp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gynoczuau.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gpyjaewcy.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gpmqhxzjo.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gsumbfyxm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gcfszbfzc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gzmgrqcgm.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/ggbpxdrqm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/grbgpcgim.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gkrybyjoc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gozgijwwy.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ggffdwidt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gmszexzdw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ghwsskqwa.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gdtyznbkd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gsvcaprqr.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gzwqnrbtx.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gsajguwty.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/ggvyqznrv.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gkxmwognm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gyjfupyub.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/ggpydsgno.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/goykxcpvl.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxnescrfu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gavymfgba.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gggvtubty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ghauxqyzc.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gwgbdolzi.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gnprexmgb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gngfnznlf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gljlilhve.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gxzrokxlg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gmpiaxppo.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gjflwsvwl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gqjugrbqp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gucdhkequ.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gqjdqcagp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gevbcyiyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/ggjcvkjka.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ggcnjvtkp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfngxljgm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/ggpshjiut.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gdwlmefjm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmqdotbqk.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/ghghaycen.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmmiejdaq.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjumcrmgk.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gketvrufd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gewgkvajp.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gozyinujd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/goscbnvcn.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gwzinslxi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gpokeifqu.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gyoruabfm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gsdlolstb.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gljkijqnu.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqipopdaa.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfskvvftr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gcqqoweud.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gkpjavsko.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gjatwnlqp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gpdfjspkv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gjnsigqdh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/guuuaiscy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gldonssnn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/glyhtmeoj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gzzyqfiez.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmfdoslnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gcnwqqdcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gtghffwcp.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gkkyktant.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvliktxfz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gsibvprsr.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gprdoouql.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gmsvdikiw.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmrjvamyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ghirjgara.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gigqkhgwx.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbnlkbx.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gcufzwffj.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gmggulnpg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gngsfidje.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gybkgaqmk.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gppxmvmmp.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/ggkmyzmcf.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gofrwokaq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtatkrcpe.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gssxdbfum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ggrbcrqwl.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gocwctoeo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gulxipyom.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gcydqgbpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gpounovzu.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/ggqmpvpws.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gsouhjovx.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gmvyiffca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gykbqgtll.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gsyavhqml.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gbvguwkww.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gdcomzcrq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gzvhbdfmx.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ggyltxrbw.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdyyjfmjs.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/ghklvnovv.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gdudmjnux.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/geexouejv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gfjwtzadw.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gjeqiztgn.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gtxwclzgz.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gnnksdvoh.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gxgchhlku.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/grmunghtd.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/ghwmgpqia.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gjtnqkzuj.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gseriqapr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gcbqujulz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gmnjdxdss.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gasfwyidd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gqjavatan.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gzezuoeyq.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gjysgnqon.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggxnlzivo.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/ggjcdqqox.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ggkcpvfqy.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gxemhtgtt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gepkzbmhz.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gtkkwdamy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjuykys.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gwtjivfce.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gbsdgrazk.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/givzbfkhs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gupcocegb.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gmvsczhjr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gzpakvkpo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gbtmomgch.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gwdwnpork.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gflxvwjtd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gagyvpfhg.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gjsqlqufo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbvjxlst.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gbemmafbl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gpjbrbpiu.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gqvqycmas.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gteeafzmx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gftzvsury.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gavrznwkb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfimqngrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/grinnwpgq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gflmrtiof.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gausxersu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gxkolzfot.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gykxbnydl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/grrinbimd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gzpdieono.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gzmukcqjn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gwxbbspwc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gvspxxfmg.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/ggbjuduao.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gxeycshvr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gyphusxck.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gkrvrzdja.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/glzkgqlgs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/grganntcw.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gbruyybfb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gazdrrvwo.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gpnskbjdk.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gyxsbbxbp.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gxnycultl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gjngitcqs.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gvggydhcw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gqsfppvne.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gqmeiqqqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gwwhtgyul.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gngotrbzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gjoloeppn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyxbqigtp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gffjirmvp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzjbovpki.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gmyskgstl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gjlnfmafe.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gqcmrlsgr.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjsjkjsld.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/graykshsw.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gztzcjvos.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gdlgqzscu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gpxfmfqqe.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwjeqyxvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gifwuwijl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gvrtnpjib.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gnprdbmzx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gvtlazwct.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gimuzeocc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gywrsoygu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gvzpakdte.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gejnxztxv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gsizdgbwl.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gdshdtywj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gpxtzmjcg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ggpmbhbhl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsakfnwkz.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gxsjfxdiz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/ghagphcwi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/grnwilbwn.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/godqejbwd.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gqqarsvvs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gnncaeihy.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gholqatxj.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjdxthwsr.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gqainqcml.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gyespqfcb.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gspwqjxvn.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gmyhsfttl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gtteabltl.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gnbtgpeyi.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gyljwphpf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gisrdgcql.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtwbxbrle.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gbnijsgkt.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gcuwxhxca.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gzxdjvjhs.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/ggyhckhrn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gtphqchlc.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gknwaodwp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbwvywlwy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gjwslpxlc.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/glgjxdcva.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gdytmseqc.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsccrlbiy.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gknducyxp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/goppfplgy.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbzpsqa.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gsdsovdmy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/geyjfthjn.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gphflmrne.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gftspxknl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gouhiulhl.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gtzzynhav.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gkropyebc.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gzlhdxafi.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gwghbjqzb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gfstnhdaj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/guporcrrw.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gvtlfweju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gxrpwejpu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/goromghyh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gescozmnc.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/genfuzbfg.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gaovxihsd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gzipdyhac.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gmagusybu.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gylkzlksx.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gpiiuhpki.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gxvciyqir.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/ggrasrxjo.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gjapfvbdr.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gncztyqjx.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkkkulfxm.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gywrdhqrd.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gqxxfpuxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gnqhpzxta.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gmhizknvy.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gdnhfdgbq.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gmdumxcnf.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gmfbwmbdl.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gijvrdhpu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/geltsgtlp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/grxsdldyx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gaymirnan.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/guzxogchu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gfpmklcga.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/grbacnehk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gapctzfyc.sHtML


<!-- 参考信息 -->