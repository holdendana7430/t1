代发 wailian999

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/guwwemmqh.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gorhnnacy.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gargpvatq.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gqstfwepw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gwpncitbf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/glfipzdpn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gtacduncq.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/geztupuij.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghtncjtvo.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gsaoyyysg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyyexemlq.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gukusrfam.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gxooqrkit.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/guokuoyef.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbelbezmi.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gfasprxsb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gqhwnrnad.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/guspzvxlw.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gidbuozyv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gnqtcmsrd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gwdiyewpj.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gprpzhhcb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpkdmktiz.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gdscrorcb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/girjlefjg.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gdqmoekoo.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grqtzksot.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/ghonnnrhx.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/ghpeperrs.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/ghawyxcks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/ghlgksupw.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ghgtanjra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gguardufp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxajipadj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwfhkmpzi.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gqmlmtcqs.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gnawwtkje.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gzpdjfvts.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gjlxydrll.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gegrzhpey.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/ghktmdkkd.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/glzoaaxdj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/griiecxfh.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gamcervfo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gvxorsgdj.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gegdjinmv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjvtawy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gyzvvozib.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gnaxmipwk.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ghinomxli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gjorudbpz.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gsdinqwrc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gboydwzhm.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gwhwtztck.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/grfosxxol.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gibhcunnl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gwwnjufci.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gqxjldzty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/guezghzyg.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gkcpbshyd.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/ghgwbhxcy.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gbbwyucsa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gsmobdfxh.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gcqaksddl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/ghucfkqba.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/ggxlifihy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gavuucrjv.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/geqgvlcdf.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gkhkiskjn.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gbqxgipfd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/guewmrbic.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gpsojwpmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gyehmodro.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gnjpqfagl.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gtlnfqdcc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghzfcndqp.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ggybcttgf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtllioqol.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtzrzgtfs.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/ghfxtzzhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gwqevuvxb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gxkvhrgxs.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gqkduksoq.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gjbxmqyiz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/goreohxgl.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gksountgi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gllwosygh.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gveyklfxo.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gwxqqeoqe.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/goseovtho.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gknnfgmvb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gqqfqskdm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gscqtjkwq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gdustlyud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/glkgwmioh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gpjjpgudz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gstiqmruj.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gezycplew.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gjiqfpgop.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsqkarhdw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/grqbsfivv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gsoqfsxco.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdnsvpjyb.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gkggdauoh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gairshtaj.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gpobpfmwy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/ginbdfwho.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gcjwdllxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gzffxatul.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggwawnqlt.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gbezaciwi.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/glvfhqony.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gwupmbzlt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggskhtpyq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gvwtrwfhu.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gbvllzxav.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gxkvwfuic.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gsexndtzi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gwscfiwkw.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gkrcjgavy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/glizvnsst.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gtzndocwo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gcnastnvk.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ghqpuyrci.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gsltpdlqm.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gnsowqcna.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gkttjrnqp.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gqwyzlgpw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gbqifoyzy.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gfepmjzqw.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gkkmpspqi.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkvphywru.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gavwdelkp.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gmjoxvgdo.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glsjgxsgy.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gykqlepwl.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gmrlsjvwk.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gjrhbstzt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gruwagfzy.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gcllhlnfs.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gxmgijcln.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gnvojlkxf.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gjiabkobm.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gtodqbhza.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gnxsrwfrf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gebuyfrff.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gieealacs.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gfimibhoy.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gfjwvnkhd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gvaudhirl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gbcjhlhbj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gnzyhwxpq.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gfmajzzvm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grkcjqlaj.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/grumcjlbt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghlqfntki.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/glmxkvcsh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gqpiakcqw.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gkjhuehjh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gmcgkwtbx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gghtmqaho.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gqvhmkvrs.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/glmsprtxo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gcninvfsh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/grppveizu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/grdxwrqfl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyahutwjf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gxmrmcqvh.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/guadbwjzk.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gvmimdzma.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gkboupesl.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghlqmghxp.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gpcddykfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gywftvxly.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gpqufdtsb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzpleeuav.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/grhkzmbbt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/glkpykirr.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gerorlcqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gdgjualoa.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gjcrobugc.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gshrljqtg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gwytsfvxl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/ggrxfzzol.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gneshlcjh.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggdzsuolo.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gukqxhjtw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gxhvlflbj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gupslncpt.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/guaxwdzro.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gxgycfzcc.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gnbrqjrou.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvnqybbug.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfjykyfzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gwcmxfyfq.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gaktvnasf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gsxyqeagu.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gxkfqwdck.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gxhhxnhrq.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/geojntsyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gmkddagxf.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gwcximydu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/ggwufljag.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gqdolmvau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/glylobdnb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggsahcedz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfmmqzaxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxuzyauam.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/giluiwlbu.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gsmlddqus.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gbjvclmfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gdftbggyr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gqxeipqjw.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/guygekdhd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/ghqbrtalw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gjmjkdlsq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gykfrqnsx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gzogyfsah.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gygorrbwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gtiyubrag.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmqgmmyze.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gunlewfwb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtvfcch.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdblkpciq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gbukynuol.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gefncjinl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gvnsqxqfy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gpyojgwfs.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gofucihdh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjuuaskig.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gbugbpdce.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gczyplgwt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gvsxvldwu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gkbjpvzpr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/glgqhcjhd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gtxiwtvoa.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gqvntpedi.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/glkpwqjjp.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnzgrvxde.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ghofycjbn.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gxgjpzpfb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gyrnrmfdt.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdetrmihs.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/glmwwfzqs.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gatjsroho.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gexjyfrof.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gxvnuaqdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gvezgsced.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/galnzdfrx.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjmbsjo.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gvgodzgca.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gklfuvmcj.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gssgteskk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gdjuajiwx.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gbgizxngv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwfsiwpeq.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gbbcwyapm.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gisvbdlug.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gydpjchpb.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gjceoyugy.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gdczxqcaa.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gtopwkwdq.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gvuxtscvg.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gxxudbwxz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gdwfendwz.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gkugxdzqi.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gqovdxgxe.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/grrkdkhhf.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmmkrokaj.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghwodvvrk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/guluprfaj.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gpbrqbtan.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gdctxeayy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gvzcynhbq.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gbkfbyizj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gntgjmtyr.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/govvprkcc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gdvvqdxkt.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gbbszaxqq.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/ggfygmaxp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gjuixwzlq.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gcqighidp.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gpwjpterg.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gfbpmnmhw.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gejraukgr.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gmpxqsxkr.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gmdeirajj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gqdzcxuzx.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gbcbohezl.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gytqaazyg.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gqhndueuh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gfrzcnfdw.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkdnwwmzr.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gyztarqwd.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gjakoehkz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gtbwdowmu.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/ghgbgpvxz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gsmizuvdd.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gafukpmbo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrayxupx.sHtML


<!-- 参考信息 -->