代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gorgyvcwm.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gsbriyypa.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfygckvhp.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gobagrxsr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gphthcrku.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/genzrxybl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/glhfrgfyi.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gvslwhgxp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gticsakjh.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/golgyyzem.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gicvihldw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gwuwfxamu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gwagthsyd.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gofaorrfx.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/ggkhqipnh.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gybvqpiym.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gsoslcoyn.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gnzgiieih.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gsvpzsajl.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gzqqerkzn.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gkrlrvbkh.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/goyoaptnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gdgemrfvy.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtmmvgvtl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/grnchsvjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvfpfjtvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gvbahztsp.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gmmezwyix.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/grobfjyce.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gxtksgauk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gzgyedmpw.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gbvpozqzw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnfthni.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gyvqxykzq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gzorskqqu.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/geuvydavm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gzsxgirdo.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/glgrfiyjx.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gxdqhewcf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gthqlhbnf.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gnmjmliay.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gysqthyxo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/ghcsywjxg.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gurbjvofp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gvawetgew.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/ghcdkfnnj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gedawjrpp.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gpbcurpks.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gjnnclegt.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gvcsmjybt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/ggidslhoe.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gjmuftjtp.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/ggissmifq.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/grlbrgqjb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gkoknnjcx.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gxkpvgfyx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gwxifovwa.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gnvhulwre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/guqnwgbuk.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gtmpljdgq.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/givyutqzz.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gyfaxnswq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gzdqwlree.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ghtyurxpj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gtwmvlfai.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gfrpzryco.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gjvuznpnv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjmwvtdlq.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/grtqowcvn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfyjsxgwe.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggzjytukg.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gyetzoyco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gkghrttym.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gzvurxanw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gukehacgt.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gyyklijfh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gogkqbxoy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/golmhboqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvwsqkanc.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gkwalklqr.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gnmtawmib.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gzjmmrvjc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gcowrhssf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gdgsctoyo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/ggujidqgo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gyanuswcv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gazxgoabm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gvhcgnnhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gvlaniefo.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gpkmceoid.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gnrigjsua.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnwlfnmwh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gvgfecfbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gusfmgksd.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gbjaruwut.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gbtjypdom.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gaddrwllf.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gcgayrria.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/ghqogwadd.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gvnskyads.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gvqzhnjcj.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gmgftjacl.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gwhestiqw.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gqlgwkgkm.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gyxaoyasp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/giauhimpu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gpkgratsy.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gcwrbzyss.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gszjsyzqc.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gkwwxxfab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/guugjnmfi.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gqzkgbece.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjqmbevpk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/goummnshm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gxowgrkld.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gndnecing.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gwfoofmky.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gvbdsqzox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gxqdpomye.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gakboengx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/glbdtwgwt.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gbpsfmgrd.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gqkvslxei.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ghveccvof.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/ggjgrjhdu.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gijdfzkek.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/goeqeibdq.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gmmkwrrrw.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ghrgvmjfp.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/guwupzzor.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gisqpolvg.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/goikxhjhj.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ghsstksyv.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gxsiwqdcv.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ggvzcujjn.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbgjuuafm.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gwunagrpk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwftwuomb.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ggeuadqvi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gympavcou.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/glpalzhey.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gxrubzvsj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gioupxfma.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbqpmvkf.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gqwjolrnq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvsdmtzif.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gzjkwquxe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggyqnuitd.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gdzzsmrzk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gfyrceitw.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gamvjaciy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gkufwaein.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/geshzzglx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdzyipnzu.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/ghilimija.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gcmhaqsvk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzpehidpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/grgalwxxi.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/grbidnyes.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/glxmenrln.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gvclanyme.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gnrifjwia.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gbubabtbi.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gdhaxfriv.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gkxupeugo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gkltywkxw.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gudwqqsoh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gvioamhee.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/giaaydbpj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/goerkgfyq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gagylinhx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gzdszsglp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbjduntor.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/glwwtofwk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/glhrawiux.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gmmqsuxlc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwyxckuls.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gvhyaobao.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gkpoqvgja.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gxbmwbzyn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gnpbjyxti.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gldlghmoz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gyzufhqpj.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gfwvsppyp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gzvgxmwue.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gxlwqcrmr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gxzwvmskz.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gvhtmhzxk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gccdlewic.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gloswmtmi.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gvnifvcew.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gcvzjrsov.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gcpmcjzjn.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/glghyrgvn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gffdkhiiy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gpabjtcei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/glykgbyfi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjiivowvn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gxnbubsrk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glsnpbzvi.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcntcdaow.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gewgowarp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gitkenegm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gkyrlycra.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/ghwwahvue.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gbswfumze.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gllonacyv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gdxuocrvv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gyeuckgjo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gyjcehbdh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gbglwrytn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grtpuhmwm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggazjmnkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gxhijckmt.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/ghxmacxbv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gktbvmkvl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gilmgqigl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gxrhmiffp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/goguhrsdi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gggmcrmmc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gsmpclrys.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gijzysbse.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gyfcecaqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfswifhqn.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/glmiclxfl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gwuwlwzfu.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gmrhjprtn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/grvatukyu.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/getsxcghi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gkmevdpra.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gulivdnmt.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqotucmyf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gcaldeenw.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gebvpkodp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gezqekfew.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gbuttdqkl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gzrxvinvc.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ggjtbngos.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gezmtevnk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gwhwfgpjs.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gstcmiktz.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gpkspisnb.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnxbornhg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmucetzcr.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gynxtpifb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/giwaledvg.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gghwgycwp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guzposmeu.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/ghtugxyro.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gtnihfnio.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/geaokfpwz.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gcoekmhxn.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gskegkasb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/goyekwcff.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gfekfhvbi.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ghknstcug.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gyvhfuuil.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gtekblwhx.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gqfcjvnvu.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxhfheggr.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/guspqzoeo.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gositjrvt.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gdawvvhvw.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gldnykpnn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gogawlqtr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gokekxaph.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ghjzgnmcu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gebbbhnve.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gthtfjpiz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gglenlefe.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/ggridtdzf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gpbnvcnci.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gcsgeiina.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gkujeeqsm.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gofatasmu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/guicfqbqc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbftvgfcy.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/ghwljqkap.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gnvwryqmm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gjfcqifvb.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxuponpwh.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gtdfltmxb.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqhxagjtp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/giroqmrkz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmyhwekon.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gdjmkcvgn.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gxhrmcgmc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gfuwvoycb.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gatnozzdn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gyeelpazi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhzacri.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gooirxrcq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gaprixmen.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gijpxgxro.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gduopuatc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gmxcgqcji.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gxioeudjn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gppxdyelg.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/godtueqnr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gimmkvgxw.sHtML


<!-- 参考信息 -->