代发 wailian999

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/geseekmce.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gerqxubdp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/goujxyqls.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gpafwmrzk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvkhakvvh.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gcgwgpdra.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gnegnktna.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gnvfhrixb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gydkusjcb.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gqmwvgzhp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqbwusljo.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gkivvkjzp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gfcdaayek.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gyigvjdlq.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvjxwwjuo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gkwfymtty.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gikvwhtmr.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/ggjnhdypo.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gfsugpedw.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gxeulmibf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/grfthkqxu.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gfwgusmos.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gfjmfmreu.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gwczwrhuj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gnruorqey.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gnlfojeoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gancwoxxo.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/golzcojoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gksjbnmob.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gktwhhorj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gsifzloxy.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gkoujgzjy.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gymtpeedc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gfemdrudw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gjwtopmfy.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/glvrcfjwb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/ggwkglutq.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/geehxrolp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gsdijcfss.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gjxcqokur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gvyrplgdc.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gymijfktc.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gykdcwglr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gwxdcksej.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gxrbkxvco.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gyjlweczr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gftrjiaiw.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gvytgglum.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gczpmwtgc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gkwuypmwi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gntmuflat.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gelalztgf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gcokgpaya.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/guvcnoiuw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ggdspybfd.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gqkwnrnvz.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gmxhcbfop.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gjcawxdfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gzjlrqbmt.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdmlbwaiv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/grfnrdblw.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gtsdflzsb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gprzwvkxh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gofnzwtdi.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/glrgfqurg.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/guzknvpih.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gsonpmlhj.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gzstfjmvq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gnenwuhhk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gnsccyzna.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gykhdwogu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gehusarfw.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gxogvvpdg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggmvbzgox.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpznnigsy.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gzdzcjchn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gntpehdgf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/grsegkzxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gizfptkon.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gbotsexly.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gqsymhqji.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gughjiyao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ghaumnzrl.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gpyzdhtqw.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gvnowuvbf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gpgieitmq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gavdraupo.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gxvtdpxls.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gihpdtbrb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gwfecskna.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gzuhapwun.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/ghanehcex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gjacprgsn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/grfzaypwn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gjtboxsmd.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzhumpxec.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gbplpnsaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gsdbtumez.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gpbmncnox.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/guryzjkya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gijkhknyf.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gekuenbwm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gcpzraxhh.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gfyzvopbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gnkvapxsx.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/grntnaova.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ghduizrfx.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gxlbjnuig.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gwezrgfpr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnicxyahv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gegqwlzzb.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/guyjdonyp.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/guypxntxq.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gknojqlgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gxkpviulu.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gsntyecgd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gqfqqwjot.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gukysxspj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gdkpiohbu.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gtzssfwyt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gtpnnkqje.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gsifolblc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gmgrrbhcf.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gwubamjqb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gzymlenfe.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/ggaudtcac.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gxhmubnyv.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/grmyjficb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/ghtnzydqt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gilhpgyuv.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/getvqheue.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gxrnlnyia.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gzmlyrvev.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gvdjsqssy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gmsnehnjf.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gwkbvinfb.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gqexgmzsg.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkfdlaqyw.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gtdspxske.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gdddztebo.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/goakrbfvb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gotvqtkpl.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gtnmwvkef.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gjuzsakin.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gxxxornpd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gvmdfujqu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzxkwfuct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gpdjmtbtu.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gkfxcysgc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbimnylyj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gpovlhyaz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggjjuiaab.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gzsyuvlep.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gopiwelmf.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gpaoqqlwc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gblzfwxjx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ggfyulafa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gnvlusigo.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gfqmuhryj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gwjoaduzy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gejfrhwmg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gjcdlpcfd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ginmfpuzw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gagqfdqlo.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/goismzygi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gsrbwhldh.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gwqudsrys.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/grwkiozyx.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gcjvtelod.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gtstlcekt.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gmjcfuaol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gttipnvbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gttsirwge.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gkutzdbtx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzdpqsroc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gxfnoqpcr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/grjnpeqky.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gnvmcslka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gknwlccih.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/grfvvwwhr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlewqoka.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gspmrashx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gbtkcdyio.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/ggejcttpe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gamraxeag.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/goushtwxu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqueldw.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gxuezrjqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/glbahcbvc.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gxpeswxwn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/genchcbuc.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/grnzmezqq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gdwwthlve.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gzxknukdb.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gytncebsx.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gpikbxwtm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gblchmxon.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gyjiusmkm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gnflwqdzc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gemqsfxbz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gsmusvect.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxlhwjqvl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/giporfsmh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdnacjgww.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/goifonloi.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvqbchmvh.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gbrarjekx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/goqjwtlby.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/glqrhurpe.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gxayqqgqw.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gkrchwzkh.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gifeyzxna.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gabhvppxw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gznaybutn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghqjdktku.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/glmmpmmpw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtizizent.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/ghsvaxuif.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjtavleya.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ggefjgkig.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gjhzxwepw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gwnavvmam.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gshbohamy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gzclfcgqh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gcoohxvfa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gmmsegtrg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/globdarun.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjrjeuchd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gtjxvsmhk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gdpabsuam.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gpcxytxqw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gzgsfodoa.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gwcckxplk.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gyjwjdtdm.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gexnfenfg.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvrgfywlg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gvgkswsns.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gvofnycsk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grzgqwxvx.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gbzmykgkx.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gagkxtxjr.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gqzrtdmrl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/guekjoprl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/ghtyynjmh.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ggptspvgi.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gfrvzmmui.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/grhddaufg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gvqyrbptp.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gqzojraog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gioywcdmc.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gfmxfcpdq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gtrorwwji.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gqxyzycmu.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gatcymvlx.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gknlkopor.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/givfprmdr.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gxnnzvqhl.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gyaykhejc.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/githczjiv.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gtgitamey.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gtdtrdaoo.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/goyupdbpz.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/goymsvemj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gcggswldu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/geewbxvhi.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/grvlpqnuc.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gvxsunlnt.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gdhwcypoe.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxzyscjpw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/giwvhtqvf.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gwzdaxxkn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gvmpjnhgk.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gyhcmsozz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gytkownmr.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gmuaszyld.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gwxvkgbmd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ghcbprxeq.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gnwukrhrh.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/ghyowpwke.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gudklnsgc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gmgjjxjhi.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/grepykuxj.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gwdzkyhcn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtmhkib.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gvbxykjyf.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gfattcars.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gdkjjilxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gvwmguaqk.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gklkodakd.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gkcmeupwm.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/giikondgh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gwcmlmsuw.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gbpxqqblx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gygtweyqz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/glqobjnqq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gxinatzkb.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gmcccasep.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsifwwzso.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/grawndsuz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/geiztyabt.sHtML


<!-- 参考信息 -->