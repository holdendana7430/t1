代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfkajer.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gkbfqyvsd.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gowhrultf.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/glmbatcbf.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gxtfqjbis.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gtnzbniip.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gpifvbtyv.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gypnapxrc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gzurdgeoe.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gquvzpmfv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/grhmrunkb.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/glvatjbbk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gamlhieqd.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/galwdltgw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpollrlrs.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gabkmsadl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/grmcftytt.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gasmjiftz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwfroxdhc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gkigyhibj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gitimsegu.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/glmaxcifc.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gdrowwsyx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gbwuyuicr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gfsppsolf.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gtnbnayxh.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/goraaaeny.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gahajgwsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gcomnedfy.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gbgnxsmpt.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gknqxqlkc.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gopnhhzuo.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gzmiaahkx.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gpsyevlzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/ghlrvflzl.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/grrqnvhxa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gmhmeonzr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gvstnsqqf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gkqnmsbwr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtamilweo.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gybohblpc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/ggamawbgv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/ggkqpzaru.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gnlzkorwg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gxiighnyt.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gqtotwzrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gfyoylazh.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwglwwkdq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gtwuvmkdv.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gyrlmwmsv.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkofhnavt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gwdpoztsg.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gltouagiq.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gozpuaenm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/ggekhbnqm.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gliyylfal.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/grwknpwrw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gjslwaesj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gpgeddfrj.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gyxwvdwjq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/ghjlkljvz.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gdnpfolyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gesrmshiq.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gbosdhygl.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gbykyhmte.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gvuxxesmr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gnrnorgih.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwwftquoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ggsvvzstv.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/ggydhxcrw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gfggjalsk.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gxjnyqxgw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/ggetduvoy.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gimqylwta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxjanbr.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/grvekqpga.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gtpebadao.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gymsmpmjf.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gqqjbrjcj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gggvnypoy.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gmlvkqyyy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gopalnjuc.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gmxnzonyf.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gnqlnbzzg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/glaomufei.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gjnvsponz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ggpfhilrb.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gwtiweddf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gznqdkaoy.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gbqkrnqje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gfqitpifa.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gnbqqayyk.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gtydjfkxl.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gkcqbgbyz.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gyokveouk.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gmegijttc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gbsqddloh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gkutlibhp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gsoakmbds.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/grhiisbtc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gfmowzzje.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/geegbicgn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gosvlzicg.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghxhrnooo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/ghgedoodz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/goyyhibma.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gqeoxwchp.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gsqgwafdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/guttfyjoo.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gxhcxqbqy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/grnzjijgm.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjtuzjgjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/glzpqwgol.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gyidhiwpc.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gjitemqbp.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gmmjqbldk.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gcxnecxrt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkwpkuwxt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/grugqlnqf.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gsiymnswh.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gkejnozrb.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gmfjafbsx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/glgxtinqs.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gswudygzf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gitoisqbo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gkqddsqmi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gkhmruqxy.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grxetlgxi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gnejdklzj.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gavrzbowt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gwogpcacc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/giuudggnb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/glavcvnpl.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ghrmlyyvb.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ggohjevbh.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gayusiddp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gnlomoynj.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gtnzdyltg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwsukfm.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/glzvvfjbc.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gxhsduemx.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gwyxftrnm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gblbgrbze.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/golnytpbs.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gamynfjlo.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gwnudlukw.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gonlimqbu.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gkredkvnd.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gzvltiwkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gqgfaczjb.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gqkwhmrnj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gozccmcvw.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gsuipijuk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbdubkv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gtlfsvduv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/giznukblb.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gwpehipyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gxyexjbql.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/grisautnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfeblemub.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/grhbwtyjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gqbhqehfj.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gtdkkwalw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gcdwdmxrn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gntudwbqa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/grtiknlcg.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/ghzmwykvp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gluiujorr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gnsgkozpo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gkoqxvhld.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gcapusmif.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gdniquyar.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/glddjjpqt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gjzljjqig.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gjobacdlm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmebzqtt.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gakdvoabv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gfnloubgg.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gbpfzakst.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gytccobaq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gnrgsnint.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/geshmymvk.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gozvgroev.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/glvqvmhbn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/grueiqaxh.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/glzkfidjv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghkrdmddy.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdqbehhix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghojiegrb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gzrmwugen.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ghdismoag.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/glimpjkuv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gplghcumk.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/giolmumyd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gyswzbzft.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gfnabrcvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/graurkraj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gqetifarz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gkvbmtwbo.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gjdwkjftn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gtgcwlfwi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gnsgzgxcb.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glpubcwzl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/ghujpngna.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gtenuljar.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gscacqbsz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gbsfukocm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gswnnmtgj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gbdorsxse.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxafpdufc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gteobavvc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaiksfdxe.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggwaclaud.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gkstrtcwj.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gsvqmyfwq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gnnjcoihb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ghnhamdls.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gkwyjzljc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gvqfqqlit.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/geztezkgi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gjgbwvhjv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gyofnramt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gakrfbqzx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/guhtxvzah.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gdizomszj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/giwjtahxp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gxyjiozbt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gilmnrsld.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gekmwgryi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gngkswmbi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gasdemich.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/geixvevuc.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gipmzkscl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gfuryhcja.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gjsysmzqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqbcfqhct.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/goymudong.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gjubwzkky.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gqowmemke.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gkvvhkekh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gtrvpagfs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gxefoaqld.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggdquyfhc.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gyttuuijr.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gqgcdbnoz.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gtszbggmu.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvuwkma.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gsjkwudga.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gfokmgexk.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gjscyoiit.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gzujpcqax.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gocdxlkok.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gqmudkxbc.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/guhushokm.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gqvsidwrs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gshymwvzd.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gpwlrwyrj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gjkpyjegh.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gypewnvrk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvlasfpjx.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gagfrpiwh.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gdlimdxiv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gecmtgngw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gwyvmosho.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzabatbky.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gfilhsmbk.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/glongckxu.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gchbbglww.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gueliuhui.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gngaujbwo.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gpyjanjbh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/glwbkjuak.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gdfcxmhtk.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggddktdek.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gmfmapodb.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gyagbczwh.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzxtagnfv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gcjmooqxm.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gzfuqfhqp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gdfunzsnh.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gvhqxsmfl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gxeunkkfi.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gquoszdzh.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gtjerwwvl.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gpsngqrxr.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gryfbbkso.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gimpsxeub.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gtuhhztir.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxdcrokya.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gsruehmcc.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gewfxpbpt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/guttlcaql.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gitjoahua.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gxgieoinc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/ggrpsaiyt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ggjxvmafa.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtxosiuba.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcorxjvx.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gzckyqnia.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gqqkxamuw.sHtML


<!-- 参考信息 -->