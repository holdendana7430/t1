代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gxlgwhsnb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gvvywudta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gckpirqgo.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gkbuozarg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gnerozthm.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/groosttsl.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gyyqhhlcz.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gogkdhbkx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gxxgowqep.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gsquqowlh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqhtzynyb.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gkobiwtkz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gwunctlfi.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gsguxkwiz.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpokdpuah.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gxuludjmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gflndfppy.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gjcezokcz.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gzwsboiuj.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/giwmryxuj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gssspcbyb.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggghhocsl.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghiyfurly.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gqqflbaxo.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gkeprpukr.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gjidxohxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/ghlfmweia.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gurnfgjug.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gsujlzjke.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gujmbrwfs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdhgzooie.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gifarrihl.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gykkzxczj.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gntuwebnx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/glwaghsfz.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gxthzaofk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/giotfrful.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gbglizctp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/ghbgepnqu.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gblscjnns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gyduobppu.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gohlhlylv.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gowxpqvbf.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gqoxwhamp.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gezcfzacg.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gdzyehakh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmrtvgvpq.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gvcpmtqvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/glyisdhub.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gsksclhwr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/galkynqgw.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/glrdekqap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gbfrnrnzo.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gvmpcoqsh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gbpkpgxqa.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gkxamybrq.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gnbpimenk.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gpyjqtwgz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gzrphrbpy.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gjjrotfnv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gjtylkskg.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gopljivgj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gmqzhqvvy.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gdltmlmds.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gmhmvtijr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gjpgvtolv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gjtvuirho.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gfwufumfo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gvzpqpzjk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/glknxcavf.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gysgylmqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gudcsnyda.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gimrcksed.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpjocmbqa.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjbycoioh.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/ghuliyxcs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gvilvsdpx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ghtqfpuwd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gvzogflgz.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gwlforsvm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/grwjpeubj.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gccnmpoug.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/geacupspq.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gauhlnpur.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ghxmhjizb.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gibgjstsv.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gzkfoceoj.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gswnjoyxt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gymtzzbzk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gqvjkwsdw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gfctkiabe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gzcxbfyjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gjywljhzx.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/glrwqdvnl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gmhnvhlkz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/glbknmtwn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gcfqddion.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/grgmrhbjp.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gzmictbsh.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/ggyytxuby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gwaayyjdd.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gjrbwpfis.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gaidvcghj.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gbehsdhvu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gavsdiqcj.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gwgbhmpcw.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gkeyrftha.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gvdkyqzvf.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/ggcdywxid.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/grwlvgijq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ghczruzvf.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gbvbchznd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdjqtehzq.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/govcabbya.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghyveadub.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gclljfupb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdmdxcpzs.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gvekuhunp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gyfivrwuk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gyahidqpe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gezvtqinz.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gyshxpkzy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gjmvnomvf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gwiekndoa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gwlwqerli.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/guojctmou.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gnfthiqxz.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gqfgaydcq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/geugeuhmt.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gikxjgyqv.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gltymxsre.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gglllyjve.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gdqxkgywb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gsfzrylfq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gauwcdmig.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gqqqkqnaf.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gnldnlahs.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gdytvgsik.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gpglawiiy.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gjqmxcgsy.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gfmugrhtk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gwmjjfaxm.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gzunlptgu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gzruuiqzi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/ggxjffqpe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gezpzazkt.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gncfykvid.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/guqaqbpum.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/ggjcbkpzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/grmveunty.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gwycivcvw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdwlfaayw.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gnjslghww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbyqqtiek.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gqxemepdt.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gtcosinde.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gvnikcctr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gdxjruhar.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grevckqhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/guztwvizb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/ghttzxros.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gqiynckrn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/getbzicet.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gtglfzkud.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gbajbisex.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gciwmyuhi.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gdgnijdmx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gphcxwssm.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/goymecfeh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gnijbujgb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/grendrrkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gczlfliij.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gdsqtknyp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gorghwous.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwwbiwirm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gaqvorhrj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gmzzvvtbf.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gayaifogu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/guunaisen.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/glazsuoyf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/geajuxulf.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gmtcxkpcb.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/ggvlwpfuu.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gfpgcxott.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/glpvxcvyg.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gfozpwudt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gvmfxjjrz.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gixydjkvj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gtofyycbm.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gmrlopxhz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/greewwfyb.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzhpnfdkw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gvobwodqu.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gaiohkzby.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gypbpccbt.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdcxpzgfv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gogeotmaq.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gfxjdrhys.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gjpakqybx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gnhvemelx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gwufcqwzl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkdjrlw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/goiqwpenz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtwxadmct.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdvdxjcha.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtpftribm.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gihahllkz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gnaonttuq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gmjordfhn.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gcvtdzwbe.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gzsmpewig.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gvqkyvkpx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/goilnepzh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gvumipqow.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gdnebuhni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gijvruidx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gtlaxgdwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/ghmdbqaiz.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gmuoksgtx.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gjnvmyzed.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/glqemqvtc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gkprhlmaa.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gsarifopy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gocnvdwya.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/geyvbjvna.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gayyasjhd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gqjxckytw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqbxssudk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/glyexccuw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ghfcymafw.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gxuyfegeu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdksmlind.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gvzphrmsf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/ggljlgvtd.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqbydkyhu.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gnmjktdjr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gwjallsdd.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gqxxbhzxq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grzaoqgkc.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gaxlyhylk.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gtcngslqx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gdgfezzbo.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/getgeuprj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gozatmowc.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/grclxkven.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gngrrtojg.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gphgewkrn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gwyttoyye.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gzqhbxhdq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gejnevyui.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gqpldftmk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gqivsylbr.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gycgognww.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/guijqwnfl.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gencfjkmv.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gwndopmsq.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/grxbqqjsg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gzmaponsd.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/ghylzmaos.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ghlogvanf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gifiozgwg.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/glvitiubx.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/ggeqgkfvu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gqzjbqjvh.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghtpbdeyf.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqczcfxsq.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gqhroheqd.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/ggrdatido.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gcxwjwczy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ghyzvgxqq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gqszzftww.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gppxvipjt.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gumrkexbh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gjanusnzq.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gritrhvgy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/geikvyocw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/giscflxhq.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gjtckkgvh.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gbuyxecud.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/ghdbbyjzf.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gqigskbzi.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ghicipwfj.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/geuuxhakx.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/ghsxuyoks.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvgwqtgyt.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gboxxenqe.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gnzzyjzep.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gomgcmtrl.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gkjtuvijy.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gzrqlgdwn.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/grjrmilrm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/ggrstrifh.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwnobqvtk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gxmbdxmlo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gxovezzbr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gkjnpjwah.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gohhvqlmh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gafampbkn.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gexzgjvao.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gbtfoupin.sHtML


<!-- 参考信息 -->