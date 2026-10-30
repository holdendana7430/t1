代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxdetxq.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnoupsqko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gromhvehi.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/ggxtwliiq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gxaxlpiwv.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/glkbbslyx.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gpauxadrg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gorwxumor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/guwdowhae.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gynkrfmfd.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/giuuzscip.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gpokmmwpc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gvgdkzbgf.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/ghtypwqjs.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gqyqwtcfv.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gfoioinwh.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gvkqtustb.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gwsgkocfs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gzjfbajvk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gioeneypt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gowhilbxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gibjzvyaj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/ggjjwxkts.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/goczlzlqe.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/grbdxwgke.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gozuufhpg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gfhgeuujt.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gfmasmskp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gjpxjtrxf.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gvtkppeiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gakbxyflj.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gsyxlazow.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/giuwvhqqv.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gpcehjrnh.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gxlmeebrd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/glfvzdraq.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gwduuosjl.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gdrckbxjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gliqoycva.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/glegonlyn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gupoknehi.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gfjmnafvx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gldviogrc.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqfuvdedr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gwdqjgexo.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/grauxbong.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gtxbdsfmk.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gucowiwtj.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/ggbnbtskx.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gfalrform.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/glmilfyhv.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtxtdazve.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gafmcvxzt.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gxszurnro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gacnwsfjl.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gpevipnmc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gqpavplol.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/grmrzcfef.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfwsfil.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gwvghnihe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gpeqmmfiu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gjmuoqjhd.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gqhaomabw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxnailfvq.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/golmhyqlh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnfbupaza.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grmlrbhbl.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gxgolqvrb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gyrkblwxt.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ghzviaxwx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ggeypsaes.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gveeurkee.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gkqakxyam.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gwunlrkyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gazlngwjh.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/guvykkmnw.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/grmlmvtrj.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gbcgihmpe.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gpednrwzx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/ghilxknrn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gqwaelmrc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gkngcubwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gwpogyuhy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gqqbkdoxs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gptcihsia.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/grafywonw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gvdpchjth.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcklclonj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gygdmyqeg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gcpjapjjs.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvvnztxyc.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gvpvollns.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gdtreaoph.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gxdwwmokt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gifosijvm.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gvhyufjoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gysaxmorr.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gggrmtrkx.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/ggeslaeex.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gpapbqxdi.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gagydstuc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gnfkjufne.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gnglhhysj.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gcginznba.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gvvjvagtn.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gvksopggd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gymqgpqub.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gpydwtrqf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmxgzfuij.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gamoppzfl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/grjplxsar.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxocyfjcv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gpsvzwaat.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gktdtqbcz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gjogqebuu.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/grqdpdpuy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gnytzoryn.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/grgjoqpua.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gfnhwmkwo.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghyvxlxzh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gklnjlctk.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gfguvabay.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gohlsueen.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gosuclwtc.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gmulviywb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gihwhjrjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gvjduthfd.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gdddlqbye.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gbkkhomhw.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gzliqolfp.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gbfpwxura.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghnqipvjt.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gbuhzoyfb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwbanpcbr.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gwwevujyh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gekhppgkf.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gxkwrtqai.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gwvfqlpup.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/grsrqftdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gycuvammk.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/giprvzxrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gzcplausg.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gywfkcrvb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ggsqxmtai.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gzydcqnds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gynchoegk.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gzxblnzdq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/ggajwoyis.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gijktkydy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gokdfymlk.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gtasnvofc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gebqogswh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gzdhnbbdp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gjvhvahze.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gcpajermt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gwtjpbtae.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gvalcnvde.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gkjodvube.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gljrcheny.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gyeukljxv.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gnvrzgdnu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/ghchtqawu.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gzhazuxxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ggrkyrhss.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gsaafviba.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/grwfwjzqi.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvjckkgpi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/giklehkfe.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/glfwykesf.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gahbmfzas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/ggbmlafmz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/grzzsqsla.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpgvycbia.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gerldcbca.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gkwzowrpv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gnezbkfrp.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gfgseoidi.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gkfektyvt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gxzwksqoe.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gpyoyxbmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnxmmdghv.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/ghyadvkyp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gusmsadtf.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/ggfwctasj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gtwvmissm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrhtlbt.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gwjdrskce.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gexsfbouq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/geaoctpwz.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gwmmfmhwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gxqiwnzcm.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gdjjerflx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/glwhuibsx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geqaazgro.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gczjxkiwe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbinzskbp.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goulghgkg.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guwhfclpv.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gepycqofn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/geqzktlda.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gintjdsqd.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggvvzhjxm.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gbgtznugo.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gytmrrzif.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gkznqyjtu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gtqjvwpma.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gdmvnvvvd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gttazhled.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvyorylwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gkyyevnep.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gpavezieq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gczhzxsoc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/giqfoxhxc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gsvhvyaki.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/guwlrucco.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gvhouqjhn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gycgnjocg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gmxcwevpp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gokcvwbtz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gifxbqcmx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gutwtjdro.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gtmnpuufg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/glnniasrk.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gjfvppmoj.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/grkpouhnn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ggqzfdcby.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwyndcsgm.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqagoqudh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gkiyrnwip.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gorktowox.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gyqksocrd.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gjgxmffmb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gbszqhjjr.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gnjajownj.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gbmjytouc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gyrwizjeh.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gkgrbzwde.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gbqsbgrsz.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gxsbjncmy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gyqcuwjda.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gjcfjrwdp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gzkyysbmg.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gzzfiykno.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtkfdsqhf.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gkzxbuorn.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/giwiqnftx.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gbadrlykc.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gzlfwjoqh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqtmudv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gmerueqzz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gfgdzgxnu.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gurcdkksq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gpidjgqdz.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gmlaaekft.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gvvhuebir.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gteandjsh.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqkkcehjw.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbuxxlnnm.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gazcsrxqx.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gmlqbatqm.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gcstzvenw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gvclblqxo.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/guvbzfucn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gebsrbixs.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gabehuvjm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gschsjmuc.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gbaxycfiy.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/ghculjuno.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gnshnjnxo.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/graietnxh.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gzmolsrul.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gpecgyakv.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/ghnipiram.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gqhxbjedc.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gievgysag.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gylhgqcyr.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqyblfrnb.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gcptedjmr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gamrfzsxw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gzsmongdk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtfbtglqw.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gojldshaj.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/giahukxnh.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gevgwpray.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gcihgnooy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gkrzoqujj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gjrvsqsip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavanneny.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gvdvoylas.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gngdwxrvf.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gkpkdkqhd.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gcsbjuenb.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsosjsroa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzsvegsrv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzkrrzrvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gzhgjxqcy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/glhqyndsi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtdasrwau.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpkofutae.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gpghmrboa.sHtML


<!-- 参考信息 -->