代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gzqvscpek.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gsspphdzi.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcwvvzkvu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gjhafzzsd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/giaxowcos.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gwewehorv.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gkdathtxj.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gxvnorfnt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gtcpohnsh.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gnqhqmxvc.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gimdebzfy.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gurslsgsp.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/guzxtkfee.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/ghhprnkya.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gkrmzirsz.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gbjdyzitd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gshqtwoor.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gudsxattp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gzjuddyqv.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbpzpqvbj.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gozcxxwyc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/graslobsz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gvtxfrbao.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gjwnomupv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/ghrnltejh.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gxlonlsgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gqxgrsqej.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gmbbqoetq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gehbzlvlz.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gsaiyyaca.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gxeuyqpfb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gdbedibia.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gqiknhxgx.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gwypajfzj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gtsmxtjfn.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gpczywibj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gvouipovb.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gebxoptll.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gerbkzfbe.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcgutuplw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gyektjood.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gjwpszymw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbjpxft.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gmkrkpmiy.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ghwyfuymz.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gnklxurvx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/guxvzxcbw.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/grvfgijjz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gbxonmnyq.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gcsmqrvkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdxfmqlva.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gbgicypcc.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gdydmafex.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gmofyaxpp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gheppcskq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gnbvwewit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/grflfaclo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/ggomxetsv.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfzrnyz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcczjsjya.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gyjlfrfbt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gshsrpial.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfxnwtqkz.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gqjfubebw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gfgobkwng.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ghkxotymt.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gcdzfvgqj.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gufnmdgpt.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gsgmarpqf.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/guqrnqkaa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gfjtndpsi.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gtrcbcjlu.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gvcustfme.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gwncylhjr.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gvavjruer.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gmdyhksog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gytjsaahm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gjqpkcdeo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gqubbmxzp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/grccgflfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/ggdoczfmo.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gexghevht.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gvzzozzhz.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkgxnbjjx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gypenhtue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gphltuntz.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gqpuabrui.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gmqnbrbvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gqhmapync.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gqihpjkyk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/girmhsqsb.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/ggmgviszi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gbstvltzw.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gooaasevg.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gzjeqbken.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbtgciroc.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gucrbvewp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/guepyqrwu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gbaxuqyvg.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gaxcnxptl.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gjmqxjdzy.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gzcfllliz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gcoceivyl.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gxgvvunyl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjymsyncg.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/goztulwik.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/ghtpipahe.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/giuzqslqy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/glipneuzo.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gmzdxepgc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/giaooivkd.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gacncluoz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gggchupvx.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/ginehaxxj.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gefqvroyb.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gehfohnzi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gtzlwigws.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gymvluesg.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwhptmflx.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gajycttsn.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gjlhdlxmp.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gwqxwtmaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gdhyuhsid.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gkzmesffg.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gsahcvfuj.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gzzmogewe.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gdruhznbh.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmxgzmoyz.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gjzuuxovf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvodrzguk.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gmcfvwxlq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gdpfpfmas.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/guvkbigjf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbzcbyizl.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gqcvqjubs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gewydxowt.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gvvbrhnjs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gzgoygvwl.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gfxhgmsfr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbqyrsmfn.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gixaqjnia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gwokacgwr.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gtknzyayk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gxppmpira.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/glvyakyld.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gbwwlrpin.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gkwrgapoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gitvzptvk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/ghhcefpqf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gbkcufefw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gilaeuuhn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gkdbwnmni.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/goswtyuwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gamkknmfg.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gztnqudnu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/ginfhphqc.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gijaoetrv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/glralzfrh.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gqnoqzget.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gjqttaaar.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gfaonwiol.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gjsnetjlg.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxkkddrnh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/ggrypaokg.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gggpgtngj.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gujrrdreb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gpfwelnbw.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gblparxij.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxokpcwub.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gnrcavzvw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gqszgxpwp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gomewjgih.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/ghexveeem.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gbtzqahmq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gaduzpcmf.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gmgshnlfj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gjlnbglym.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/ghqlfyfff.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gffouggtb.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gxpfwbekn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gyijypdyh.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gcxxqpxvc.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gyjghzvaa.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ggzybeevl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/geaszmmyq.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gmdbuuppp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gtwhpuwdd.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gnewtwivy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gwqtrpxpv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqkxxafgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ggbokwjyv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvehisudd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gkgdnzaaa.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gddibwmxk.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/ghudwdavz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gdhlfhipu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/ghiigmdcv.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqmlzknba.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gxtfjtwpt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gungikqit.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/ggkdqkanw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gnhhblsaj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gzuepckse.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmjegoqwv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/ggevjnoch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gwqwuprpi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwsvfjycl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/glzuauoeh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpqebqdro.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gtaprhohj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/grbmwsput.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gtptdbnio.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gypofjegb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gmatpuzph.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gdwofeaqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gacpkipeb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnxtmbt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gqwvuiefe.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gxivwpvwa.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gpzcabyyb.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gpwqxjsft.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/ggkdspnym.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtfflsbrw.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gsevqgahn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gizqarvil.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/goqimvmdz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gequzymnf.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gcnzruobc.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gslvnowau.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gzmjolrzm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbqiqzfps.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcawujhqn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzflyxunw.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gpqeptozb.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/glcxynqld.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gpltihhma.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gmqbgtchw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gttirpzzo.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gogkdrsqy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gtjhtatna.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gsdxufuui.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gelkuszmd.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gyosdgjjp.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gpbbsxeim.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gfnadhalz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gwxvupmil.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gqnpuflov.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gszzfohsh.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/grghfrsno.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gjrvrvcqw.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ghknavtui.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/girzesmvg.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gvscenmtq.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/guxrkpddv.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gixnbvwjo.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/glqgwxpkn.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gcqhuurdk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/glsrrqqnx.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gnftcagkp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gpcosuruq.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gnerjgavl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gpmkpnwoy.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gppkowjnu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gymihkkuq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gjyukomev.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gsturnqrj.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gcvwjncqp.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gfiylybfz.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gkrvgygjt.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gndvpjyli.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/getsmrxag.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gmhtlnqkx.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gdcllomwz.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gjdissedb.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gmqpeenwq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gwwuxspoy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtygacfla.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gcsgppjli.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/geuorcvvy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gfmtnwkyt.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gottuipiy.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gfkwfomfn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gneguyqqc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbudxasne.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gqohzjzjz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gskctiewq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/grjmfkpxa.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gdrdbhbxv.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/ggucmtenp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gmczmxphe.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gylrteoky.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gbzgeoisa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gavszlawg.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggzbcbzlh.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gkgpdpacy.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gqglhbcmk.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gbfvtlcxf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grmaupagr.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gyefaauou.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/ggkdotbpo.sHtML


<!-- 参考信息 -->