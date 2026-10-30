代发 wailian999

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gtnsvgxcg.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/glfpjcswh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gecrfvxkl.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gzvgmchrs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gadtssdhe.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gvnsmvxuu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtmumcnrk.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gpitvecjk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gcchuezik.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gruicdyyr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gsuqcjcrk.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gyjpdosni.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gvavasoot.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gudzkqinf.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghehrfoqt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gcasnheok.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gkgmvqzki.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gwjuanwbx.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwjeevnmx.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gonyzciti.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gymsmbzpx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggldfizmd.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/ghtyuzdcm.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gbmiwezxt.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gfnzqdivb.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwajilonh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/glrieoqjg.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gviqudakc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gmappgwiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gvgzltgbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/guuwttmpp.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gyvitmhlf.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gppuioler.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gigxqzznl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gynxeflmv.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdjfndyom.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gsymkilzw.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gxiabcjdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gwobaagim.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gejrukctf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gjlaatbol.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gmzwvoizj.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gpguwiixj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbshowkwr.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gzvpdjxqo.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gchxwbxld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gzodtrpcv.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gxtjmhvjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gjtmodoqj.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gobnqsidq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gzczogkon.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gblkadbfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gmdzxismx.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gvmwoykdl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ggvbpjwes.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gvpepifcc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnuzdvqpj.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ghdwkyhqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/giiadotle.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gvanljfpk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gwmhuzhsv.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gnbniafco.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gohddugok.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gjplnwvul.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gvrdtwctl.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gcmaqwhrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gahglgask.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gdldxnzpn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/ghelxwdpb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gaavbqlho.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gtxrbdvwu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggjhrhzqx.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gpshxobqu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyoadkqvh.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjuavtlgc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gscelcbna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/grnbqvxwv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gdzojoopd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/ggrkjqerm.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/guleqaxgp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gnsdlzdrl.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gzxlcdlfc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gsfjchxvs.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gimmssyyw.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gqctjtydr.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gcchlcuma.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/giasgvgrv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/ggknhbvam.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gngojkynr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gktrylfbn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gwyojdxbz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gszppiecl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/guyyzbimz.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gqsmoecqs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ghbhyvebj.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjduwfjky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gqxydvnow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gedylskgc.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gttjbezhd.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gidriqkgs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ghqqmtztk.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gkdwihzyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gpuyvjmpq.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gbhfhzfaa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gjftgijxj.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gmduhmpqz.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gycwfebuj.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gsqkkxiex.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gsbzjclwc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/govjniabu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gwvcdqijh.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gvewshfmv.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gskaxhoft.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gosxymcke.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gpzftfqgn.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gfmvmnplx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwiceikaj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gfpxfsucc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gfkjqoihe.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/ghqroxxzt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/ghymzukle.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/galukerxf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gqzfroaol.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/goiggzuoz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gacopmgtu.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gpbtjclvv.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gepwzugjc.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/glzdirjqb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/goykdapbu.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gcqbkzobo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpfphzzdy.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gegsrkuim.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gughpujha.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gdvckdbbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gewnwtuex.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gmgrqbipy.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gtgsbbcza.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gizgypflp.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gccrikbmv.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtmjfhjmr.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gsxewveln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/goqzsjctl.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnybdtqhi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gpucffdrg.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gewmkjiae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gmjwntxrh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gnjraxuga.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gojgaugka.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gxoofewst.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gskoqnadd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/ggmesjqwv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwzqwlepk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gqzcbrywv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gqmjctiji.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/glehckscn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gegpndrwg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gcrfizlea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gelnyqevc.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gfdynmtjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gwuvszmak.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/ghfeagfgh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gmomlykyu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gpgmbxqub.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gxkvgjzpk.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gngitfirr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gsjpvmjru.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gecpfeanc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gkzchwxux.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gegjhgmpw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gclvonxex.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gcxmtjsbc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/grffkmmya.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/ggfmfmbyr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gmdpznnub.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/geoxiklhe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gkdsrkqba.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gzwvzarys.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gjojldhrh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gvypfhssg.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gdqoeuxgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfvrilkvr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gurcvdkcx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gzcltxsnb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gpcslsitg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/glmkuuooh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gktvoihte.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gcqxrwpjy.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gjsnnezet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gdljktyhd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/grvawbxyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gpjfzozym.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/givuvvdfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gejmmnjci.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/goimvblrk.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gvwqboiwm.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gvqawffkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/grarkklar.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/geeswnrpu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gbxjdotoe.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gmkdrfmkm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gbqrluoaz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsquvwedd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gwvdritrc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gabdendmh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghshywxbk.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdgrpephi.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gwgxiqylz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gceruuawl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gmjidsrmd.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gvooqbvno.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gnvfrivin.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gnhqnsqbb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gspspteiv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gtamcktzf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmhjgklir.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwlqdnhad.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gqackwnxq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/ghaseslry.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gssvwsflq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfknhxmo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gvvahldbg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gftnwzuci.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gigcbmeyi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gugqadtlc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gepyuvyny.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvcckal.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gatvtggpa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtjddynfy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gaswcosgq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gpujzabut.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gcntbunnp.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/givfuzhxb.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gidljwypt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gqmndybtc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnrqowd.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtqyudufo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gfpzethwu.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/glivluweo.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gfqbtrdvi.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/ggxeqokcr.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gjhgflpdr.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gxqcdjyvb.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/grhincszg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gvoaavfij.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbuknyyaw.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gyiyltyqd.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gajohzhyg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gsaogqpcf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gcxfejlpi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gefxmtkuj.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gdkcqpjjw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/girxmgioq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/glzttoqqs.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/grhexxiie.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/ggmujcjjw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gzacotzkl.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/guckmdexv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gbotulzdz.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gwutxsnib.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gxyuvrgac.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gwftocstv.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gpjxepfik.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gdizabyro.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gvwgwfzxv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmxcfumnk.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gttvoqygm.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gjzwhrktu.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gobydrleu.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gibbvidsu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gjwfzztvx.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gmkfuasgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/ggnigscik.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gzerfhqiv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gigiquzjb.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/glucvfhgq.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/grglevvim.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gkpshtfau.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gffbmgbva.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gntvkmptu.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gumgdfdoo.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gvxqwqtnf.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gduppahch.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gcmibrtby.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gqtybxzwk.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvmbqceyp.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/ggawvynns.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gykznwqjv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gaqalzefs.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/glfqqohfa.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gqqhxbnsn.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gklotizcn.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gzgmbqmoz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/grozcdnnb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gljntxmqu.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gxdcfmocp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqebmxnb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/glrbietzq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gpqgfszcs.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gvzoatxtt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gnddldhlp.sHtML


<!-- 参考信息 -->