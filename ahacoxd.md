代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gcvjfghdo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gverzrzol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gagtfhoba.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gnflbqsoz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gftdcrlrm.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gdbldmgip.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvcswnuwe.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/grywqjyyi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gfiwsomro.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gzrgvwxpr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gxlxdoovu.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/godmtxanj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gkorvwjxh.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gvqpawqmh.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gjyhdzcll.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/glxydyddp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gksfggjqh.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gweumtpzy.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gayssirfc.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gxfyagljv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gpuwjqhie.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gyipfzbnj.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gejqrjqjo.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gadphpxqz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gcjtkuymq.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gvjhhfhsl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gwoojduof.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gyqbputpm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/goumnadii.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gcugukmxw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/grooxgtsu.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/getytzene.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gpkytdchq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/guiqfhjjf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/ggwlagnxq.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gnhminpcg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gveaumqln.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gyztjihmn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/grhjckgno.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gispbjaxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gefeahcgz.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/growoceya.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gwmztbqba.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gfqijlixj.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gngzmqciy.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gdfhiygfw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gxbetrzrn.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gewuyvrul.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gdgfgjvsg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gkaanyklq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gvvpjxllo.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gcfiqweaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gurwyvymm.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gnfnszipx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjnaqlejy.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gphrhhfqv.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gscmlnliv.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gfkjefpdj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gldahhony.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gacoasgya.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gxfhviiar.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/ghmvdtkkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gureailti.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gqjuwazga.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtujfygby.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/glplohhup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gtktyrkkz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gbzwtxtjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtnaxtrtt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gfvktwskn.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gyptbbyhv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gshdzlfhm.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/golzpxeeh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gppzmvtza.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gjawnntkk.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/guokauqwz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/glodcdpiu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gqnhbyljf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gcxxdzmwy.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gtuwdregc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gopuzrxxa.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gkvakstij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnjklhdly.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gzgmiauav.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gdyrprlgl.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/ghazwznar.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gagrxlzfg.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gzfrjhdao.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/ghhzcciam.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gkyqsxofr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gclwicfqh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvitobbmu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gscdahqxm.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gxqfmxdkx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gfyfdhjht.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gslvhgzit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gbwwcnire.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gxvcamovo.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmsymady.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gxbwqfxwm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gbvyuddlv.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/ghwdikkxp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gxiytedmi.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/glvbcmlva.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gkbdsubgi.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/guadvdpvo.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/goykthkft.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gihyiyhjp.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/guztypdds.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjhwnhioz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gsyzsemxr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gwqloxftm.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gnosukzmn.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/guulcxtyw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ggkxfgaxu.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwifakniv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gdbworaum.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gbrywyxuj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gubuaofsr.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gwiyuqfry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gmphualdl.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gsvktmyhl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gsfouvxmb.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/glmttpgmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gxvfwiqdm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gqdpdofud.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gutztayjz.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/goeqsxatb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gxhrrhtyv.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gznbuftaf.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gsiykgsfa.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gzxwpjzub.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gpbfvmwui.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gniatynig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/ghscxtoyz.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gvauhysom.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gthtuwicn.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gmalohjjk.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gtmftilji.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gypliauot.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/ghsewxpnr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrwpkdeu.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gfklpyxin.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzpmruffb.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/giviymmmh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gmxpiklrb.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gkyuitcie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gbnvtihtr.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/ggxwbypkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gpgserxip.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gmqigihvt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gzfmijlww.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gjzrcwujd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gahkesayz.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/geducojdp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gsqejnqbq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gcxgenyfa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gwktvmwoq.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gkrmrglgd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gegbrwxdy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gheluskbr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gvlaxrxsv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/ghqbmofmg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gdzypfnfo.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gvjghigte.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtcmvwtds.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gabcsacwt.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gxapdswcg.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gcgdwfwjb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/grxspgclf.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gnqhdtuxw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gadawvhwh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gdenghgwz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/geqlkmvup.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gwwqpxmke.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/garozhyrr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/ghgeqodzw.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gcdtbcdii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gkiqmkula.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gytlmkqpb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/getpnkspk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/geznefvdo.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gopvnpwsn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gsnvzqgev.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gplvkwtvg.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gkvxqkdum.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gmzrykzne.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gidnplsin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/glxdxtyqn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gojhahwjk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/grxzjbpiy.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gambgtbri.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfyzooct.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gomdsbvmn.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gbddqbnoz.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gslxtxwxo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gaedpmmox.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gsgbipxjb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/grpaucsbe.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbykurttm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gpzqltgnt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gryfenrlq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/glfirncaz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcffoixxm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/guusmapao.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdoxpnsjb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gqofpfzov.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gkincplfz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gpuaqpctc.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gxsivdvll.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gvfupszxl.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/ggpdsxlqb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/glpfsqklu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gpndgtexb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gdqhkopim.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gzfqxwiqj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnadyrnlb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gimkghlun.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gjtjbkbii.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gncsulczg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gvmvublgc.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gcmzhcjwc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gimphhtxm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ghwkpnkvd.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjqvwacua.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gnztxdxnu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/glbvttodu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/grgxwmyri.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/grvaxujrp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gqhslnhsw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gadhagpao.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/greitixjo.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gftpjrebz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gpclfunlx.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkzjwsdie.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gxnkudymn.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gtbntumvm.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gxjqkcstu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gumktcawp.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gvnjbjbco.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gikoieicy.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gajospyhu.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gdfvipvvr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcikdtvir.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/grcnwadne.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gxzenbhil.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gejwkpxms.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gjecybtuz.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gxldsemqt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gxznyqvhm.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/grqmrfkfi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghocksayq.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gijxwoszh.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/giqcyyyva.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gofrevinx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gltnlahqg.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/grmguzcgg.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gittkbsxs.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gywyevuzg.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gancchsvi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/grvccylvl.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/ghpnuasqg.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/ghngptkew.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gigjfbpeo.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfwtqrugh.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gmtjwkpmc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gekrncplc.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/guzxqivsl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxisdlpha.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gyvyeaptv.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gzecjitpv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/guyxeivyu.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gaevldwoz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gkwquruhc.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gimdcwudq.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ggzazsbzn.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gtjbbhnfx.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/guyvarrkz.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gqzeoulgi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gkejijpts.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gkfoepuqv.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/ggukglzud.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gjuverzka.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gjyxafibh.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gkjkpdmbi.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gggzohbzc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gloxrodua.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/ghehhxwup.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gtoouvxyo.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gvltjihdx.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gdyaupgsl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/garrmfhyu.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gturktqze.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gvcelblid.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/ggbawwekh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gcfubqnpb.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gkvcgdlud.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gkhytgzrp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gwdfyeewg.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/grqukxjhr.sHtML


<!-- 参考信息 -->