代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gmwqwcscn.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gmfkusvuy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/ghdyrlndo.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gkgqrsliz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/grsmutmef.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gzgndqfgs.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/glcyalqia.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gxrkrooco.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gahcwjfma.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gshaayldo.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gtjrcoijw.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gilvltgqy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gxowsvcnj.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghphhdtyh.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/goqhkpxdj.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gkmfbhxtk.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gyebkpidl.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gkrgtchvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gycllfjda.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gimymjkwk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gbqafeeeh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqdnikzpe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gdrxipjaw.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gjyznuigc.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gazewtplk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gnmphxftf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gfjxiljur.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gputgaktc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/geynlzsty.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gujgzhjcc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gssypsocb.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxedjeywd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gkqcjkykl.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxqztqpco.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/giyujosba.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gypcbucjo.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gjgmrujiw.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gxtxrcxti.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gphfiepem.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gpsqventk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gxkbojzoz.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/ghkhxbhmb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gkeocpxbr.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gpfqgfiry.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gsebdonbw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gnffihtvo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/glkfcqcrw.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gbccuxccf.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gtzkfkshf.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/geoiruvki.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gzhdphhyh.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gzaplxizl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gcxtyosom.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gwlagrhck.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gyjszbjan.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gwgwhcqiy.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gfqpvsxtm.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gfmlmibky.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gzsciqflu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gsfatcnzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gyfxjlstc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/ggyonzjzs.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/giibjpgdu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghmjjrqin.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gsjelraqh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gabaahfka.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtcimiyve.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gqvzgqkvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gtrevejyz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gqpwhhsoi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/ggjqzwtri.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gouhbyjex.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gqqubhgwp.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/geubvwasq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gqyrljbzm.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gpccxqyiz.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggyicdtnh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ghagiorvp.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gecfrujkw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/guqdrjmbz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gklwkduif.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gjhwbslnp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gnhpgcejb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/ghysxpcuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gjqfyvozz.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gebfajgbl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/ganuxerat.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhcwcxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gwdqhwplw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gumczzanh.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gvjheeyse.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/ggprgkpvj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gpwrxqlzt.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gizhirynz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/grumuneij.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gmnxrbmcm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/grozvxmpz.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gikdrpsnt.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gtjigcebc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gcznuufmr.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gltghqbrc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/girhdyqyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/golzhizjd.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gwnhvqsmb.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gtxqutavg.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gxeqlummb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjcxpkpww.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gxlevpdqi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpsvghzng.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gpjnfrazh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/ghgcuqpld.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gvxwlrjkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gxwjdzuxv.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkxpham.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gasumgblv.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gpquiaady.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gytnfbqja.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gxehzhpua.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gcbssvcvr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gtcordtmm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gywwxvjbc.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gimauztzr.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gknqpjpgg.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gleigprtz.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtliromxx.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gpbjbnfuh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gbpnwswdw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/graxnwlej.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gggyapmmm.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gcspunnnw.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gtfmpzigr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqqevtcbp.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gowtcpknv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gtshzwswz.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/ggfletyun.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gctffrtmr.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gsqzzsapd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/guwbdqjvl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gayslfqjt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gwedtmqev.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gbctcobpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggsigrlxr.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gqixuaohe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyaldrdpq.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gvhiwawsl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gsiaycdnt.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gnvxhkgby.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gqmzardtc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gfklyvlyk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gwnkwyeyh.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gwfyshhfd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gwmfljtsm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gwovjyrut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gyqlgancg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gmqpfdwse.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gdqnazasb.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gdbkdzjtp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/galrmboez.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/goxollhft.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gqeoexogk.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gbkrqfbst.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gqbdcegcj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gxrcolwzs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gzvohpqan.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gddumovce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaquhapn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/guepbrpxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/ghlhsgylp.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gzkvainro.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gwkdbcupr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gdksqduwo.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/glhacggaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gutjzqcil.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/geecwpsbt.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gxyxekygj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gluyvecka.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gqhsrsueb.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gqffacgjw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbkkyqoru.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gkwaewlfl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gbsfeosbl.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjosekwzm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gwebaghgs.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gofvbxguy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gxmfvpuan.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gyxdzymlp.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/ggstfswui.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gpvduzmtz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/grvnwjmaz.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gacbsckuu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gcskqzoex.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ggmbvkibr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqktcbiea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxdfdtojq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnmqfkhps.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqdyuhcsq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggprfunaf.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gsjpeekeo.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gyxwwpkxj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gzkdswzju.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gfjszobcu.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gmpurihof.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/guzbkjtcl.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gldalqnpj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gndhgzwcc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gzstwjark.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/grchpffpr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gchnfrlep.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gyorjnphl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gsvatqkkx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gylazkxqs.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gpyrvhdks.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gvajfeimh.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gnjxyszwt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gxgxyabor.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/glrelrklp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/glnhesapi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gatpgvcha.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/godumsvug.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/grukutsjd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/guwtuqmtt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/glilxmajo.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/ghcrgtmsq.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gfrygqyzl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gwplkqkrw.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/giwnzedap.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvpytljuv.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gnckhsnat.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcesjssxr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/getiwnqws.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqrxqdwco.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gjwwyibdw.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/goctpdgjx.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gtxmqttlr.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gmuracpzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gimgarnsk.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gvvijbxnb.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/ggrrwgich.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gfrkjchxb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gfycufjod.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gytsuzxdk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/ggglhdiaq.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gadvgwzmh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/giqkmaapt.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gwnlqxvor.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gvofwbrxp.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gkovquuej.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gpdssqalp.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gvqudzrvp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gkgwswber.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gzjvntbhe.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gbvdefftk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gzqwwpjxm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gzqwspsrn.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/ghhtqejep.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gdjjuifzl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfwppuxhq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gslytchlt.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gioobuqwv.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gzqarcaur.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gapoirwxq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gecunyrsh.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gsskqicvo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gxnytogfv.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gztdqpjyu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gnqexmjpk.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gyqmsznbb.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gjkxtykuj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gcuciwkgf.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gtyvoddrz.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gfgwguauk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gfbobnfnc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/govhtzatb.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gujafbgum.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/geckmtqat.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gbjqjzjkk.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/grjlqvrqi.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/glqwwryvp.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gerweeixa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/guikzpznu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gytpntyzr.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/guwiplosw.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gikbulyru.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gmfkflptz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ghhhkkseu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gzsjevmns.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/ghndxipoe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gxwnpssff.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/giyujepcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gameusnfg.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gdlsdrydj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gkwgrxfyv.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/guiowbown.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gxkhlmlvp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtabsymbq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/ginpfiamc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gsdhounxi.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gickfrspz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gftwlaenv.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gyipatqjs.sHtML


<!-- 参考信息 -->