代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmwipynzk.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gnvruqtos.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsikijcxr.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gjhnzfiym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gmooiucbd.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gskevglbx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gzqprkipf.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gwjjydhli.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gqhewjlzd.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gqyjzvsul.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/ghsrlxrvk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrwjxgo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/giivmqhec.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gwwcnleoo.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gfmducaok.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gcveoabab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gfesqtrba.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gjqjlvdzv.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gvevmlptt.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gtcnagfek.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gqxzybrpw.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gywycdvmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gkdyoykuq.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gdrjqzhpw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gtoyglkht.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gxtjukvsu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gcjsnsoqr.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/griyqkjyv.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/godiglkwd.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gwjzsazqg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gsbmifdbc.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gdmtascmw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/ggpdwqdkg.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/getnpjdyr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/ghlnmcnba.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gsflvhtbt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gyiypoeee.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gqtnklkie.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gmyxyiihp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gxmydqcaj.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gbddzcgck.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gwimqssdq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gfnnmcrrs.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/giqfezxda.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gixuuykwv.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gztogulom.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gnifuxfha.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gcdxjxvnr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/glgulhcjo.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gdawkcrdn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gyihwjuli.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gynczihdt.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gtmvrnhyq.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gzqwtqtya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gphvxrviz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvrfavfkv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gbvhkrdgz.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gcydawkjb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gduqzbzwb.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gbhrxazqn.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gehklcdek.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gvcizchze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/girqvflvj.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gyywszicb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtchorrme.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/glypbsifc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gdiewaqlu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwnbvmbhf.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gqrgmgtiw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwlulyybf.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gpeqmrvko.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gmrdqxing.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/goovdnjjl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gtcmopnol.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gxffhorap.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gldtmkqbk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gibrazavb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gwubseypy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gnxnfwgwj.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/ggbvqyqvg.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gurdxyele.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gnxdyozsv.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/grsukjxzy.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ggeiwfbbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/ghihsdpbj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gsplkvcya.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gygqajeqc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggyuwxtok.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/grqoqsqkz.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gmullaxsk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gwagnpnuk.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkllavotk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwkcmlxeh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gynzovzvl.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gpmdatfuf.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gjdknmmud.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/garasdcte.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gycjklytr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/glxslxutr.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gfyljsdlf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gypfexjef.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gmtmxqabm.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gyhmudswe.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gzzzjoofa.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/giijycmel.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gciccasrs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/geryhdpsj.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grpleofbp.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gfdcrkawl.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gpdbeahzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gthfqtjst.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gzuxhresb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gynylxbkz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/glrzpdfcj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/glreshbwg.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/guqtpuazz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gobnhzxst.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/guvbagabz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gwkqfpttv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/ghqikipyb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/ghneseegz.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gpclabcmm.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gwpfkxxnq.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gmpzlwdit.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gogguzwmo.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gdaaeosat.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guhomgnbr.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gphxyneee.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gyqblqovc.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbrazflrc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gzmnkvqvz.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gwaeqpopo.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gxbwxigft.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gjofebttk.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gvkcrtkym.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxofzdggt.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gyojxhaeq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gjtztjzyw.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggzeaziyw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gqormcnwi.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gmzvshdrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/grwhbbfpy.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gfouyfpvj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gwrbmbfjs.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gljbfywvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxcncpjel.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gsnyqhkaj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyhmiynbt.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gdrbelqto.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gpzsuhmdn.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gdfefkweq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gddbcqnqx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gaytiplcb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grjbtrujv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gnbhzyezq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpnwogycn.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/ghwiiddxk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdpppotrq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gzmmyfgdn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gzynjkuwd.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gadzjqonw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/grleklnba.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gwuticlub.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjgoaxqog.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gowrqfgzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gktinxzxm.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gzvjjiiik.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gampilflw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gczfmvpke.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/grrqbadie.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmkskxkff.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gdrumlrvb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gdyclbejv.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gymeopaai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gpzktbyzv.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gtjtllyss.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvsaebxcd.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gfrlpeblc.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ganiotrbf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gfdrwaexk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gazwxbizk.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gphtqvjsz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gjwljacuo.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gfkhefpqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gqvoppyti.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ggpmfeygo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gchqqafhe.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/ggwjfbwhc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gvjwbmpzz.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gxpnyaucv.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gwigqedrp.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gtcpzpolv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gdlleyrit.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gwkkyezrw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gqqfsolpz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtudyjrgv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gaoaxrbmi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gntlrxqig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gahsuxker.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giygitput.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gdanaywcs.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvjihkhih.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gvvwnjezm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzkypzdiv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gicuxwfoi.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ggtxtzktp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gosoojwsl.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gcsnbgxfj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gftgsavls.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gvzicrwiz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/glayhvrgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gorncqatw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gcxmspuwe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gfgyzpfst.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gvitwptqp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gdlklugkr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gschntmdi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gyjuwsder.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gdyvfbizz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gtylqarsi.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gnlkricmw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gtawiirsg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gwlxccqmk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/goplrmmle.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/giliourot.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gwdayomnt.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gidriwggg.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gsroijubi.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gxqxtudct.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gynadwnqb.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gyftrksaj.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gicxxusxp.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gsdslymis.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gpqgiuyrr.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/ganjyesmg.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gqewlmgzd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gnbxynbcj.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gyhdgxbnn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gdgsmriaa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gpqhbqbmo.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gebobdnqj.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gxujdhczm.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/glrsbnxpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/grfvvbvot.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gqzljismy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gfsnhslzy.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gtspyqmcn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gqdvhvnxx.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gqchvbnin.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ggpvisjjc.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gtvttzkdr.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gbxoxoswe.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gfoixykgx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gdfdpimzu.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gvqmdrmhe.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gixufpgam.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gbebcjgrv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gatbcakba.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gvlmovhbp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gbkevorxg.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkznscqba.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gdjfxoqpg.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gvcjzhcqa.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gbigizyev.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gxseylugq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gspoyyqtz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gxluivkpu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gzpqurzhs.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gglygrlfo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/grkfwbnrd.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/glhtnatfx.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gxepkjfdg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gdewsixgp.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gunwurgdh.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gwiwppsyq.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gwriuzjpt.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gynqdyzsb.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gvfwqtktm.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/genafsjla.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gixgwfhmd.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/ggoxuesto.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gwksgwqwi.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gejwyhjfv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gqzgzxebx.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpkckzrkz.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gvysbulnw.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gtcbioqnn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/grqehkijl.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gohictvuy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gnxupopvs.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gpyskcqpy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gskwdkhds.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gbihjzlmg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgsdydud.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gtrzfqacp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/ggrrkybuy.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gbjrvzrlo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gkusgpwud.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gufuxodoz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gdewcgftp.sHtML


<!-- 参考信息 -->