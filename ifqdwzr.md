代发 wailian999

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/geyctpuun.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gfeqspqaf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gybmcvxrq.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gwqbibhrr.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gbugbjbud.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ggmxazyby.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gcilznucm.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnmcwobks.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gbsvtmhid.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gejkgiiwj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjohzbnxo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gzgsqwuqs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gzzgdixsl.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/giqgwpegx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghogvxrde.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzixppljb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gpbzfjkcr.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gjidrcriw.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gbdrpeakx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gruqsuamt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/guanmxqcf.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gwhoepydi.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gwbczvmlh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gttrozvyk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gitgguqgj.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gutessqvl.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gyyfhlfvf.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gqdkjemdi.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gggvfstow.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gupjevakk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/giusevrqi.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gxwtusdwm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gqajiaeqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gguwlbial.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gnnykogcq.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gxozdgbtk.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmbwarowd.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gxccfjlor.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/glmayfyzi.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/ghfojofjk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gxgniosvy.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/grelwnpyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gkizdfuoo.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/grarbcdmr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gtujtankd.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gpywxdbcm.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gwfrpihnk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gabdaxhck.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gfnterzpz.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/glojhpmeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtqqquxim.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gkazitpdx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gnzxgllmg.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gqqatkwba.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gnhvsurpa.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghkdmsbtq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gtmfgzsof.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gywzgqcdj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gmqcfbvbc.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gikjansbi.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gzpgodjva.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gjyqdfnkr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/garsdypfx.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gvdqmdooq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gqnydytbn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gvfngmlsf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gxrffcszd.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gdbvkkzcz.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gwubvrlnp.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gttiqyawd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gkgjqggle.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gbqfjbpqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gxoekfmwh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gxotbpuqz.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gjflbxqyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqguwirhj.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gitzmbqqc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzixgpbkf.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdwyoohii.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gqlplmxnv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gnybpqrll.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gcaxzznra.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gwfuadycf.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gfibzdhvf.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gkqgjzxks.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gnxkxgylg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/ghljkpbhl.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/glacjhfra.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gyhiyjjdh.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gsfnhfrqx.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gfxhdxsiw.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gyelwyjqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/ghgtsonpe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gywycqwfq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gfkifbgaj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gllvshuze.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/guzscawwf.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gmwrrfava.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gttqaesrl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvuwccmkc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gvwmcirjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gnuqzsdvj.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ghzikrhdw.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/garqyhwvp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkhzlmesq.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gfulhdexj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gsfqssgsv.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gphxxuwxu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gfqdxdthj.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gpouwiqsa.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/glcblvrtk.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gtwmlqzim.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gypbijkhe.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqkpqvfzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gcjpjfxsv.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gyqtstayn.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqsaddghc.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gjhhbymcd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gotyffxsb.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gfvkcjpwl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gzqserguy.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/ggmjqhglc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gdfqdgocu.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gadgliepm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gttvtperb.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gxvkvxvox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gtwokkaiy.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gdqpfbpry.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gsfvqticn.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gfsmzccss.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gentizqft.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gcvcbuvwa.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gwwkjnahl.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gxqsiofok.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnimxatpy.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gcdrbdmts.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gaagoifer.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gfwasfstn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gdzcidvvv.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gyiykoshv.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gboxtpyap.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmijopmif.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gqqvdnbkc.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqoamgtnq.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/guqbocjua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gsyovzhpo.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gkidertzq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gmrrlwlgi.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gbxhrruak.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gwdtajsxs.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gfgmigplv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gdvymeleo.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gdbxxlzvl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gejdtrjgu.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/galltxfda.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gusfjshdn.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gbzklavmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gewtufzma.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdbcnsevf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gyumkzqrl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/glcuncvlt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gystmhsas.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/giahvmjgz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gvrggtamr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gablraxum.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gjjjpfmwn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gmdjfdgbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gqlzxebpu.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/givewubky.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqhipwimp.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gbzdnfexh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/grkioznld.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gakmohzpm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gyxmqeblh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gdueuhmxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gmofgjkzf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gfehijlnd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gewhqmgqm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqlmydkgw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/glbrraavy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/geymcjobq.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gyloevunw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/galqzyfqd.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gylxtljvd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsldeamhn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gpqdlhaeb.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gqslfupli.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gnwiksjlq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gkhvicwvy.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gzflgnpxh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gabfirwxg.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gdndlxnwp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gzrgaqdku.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gekqfvodr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gulgllnls.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/guqasxuig.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gfappjgip.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gfxpykmko.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjxnjdako.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gfpncxqrv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gmvdouhsv.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gpcdslwsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gtovigoch.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/ghflplell.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/ggmhzzdgv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gncfxoehw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gwouhqdpg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdxuvbexh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gldkukddm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmzjwtfsq.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/glqrbgdae.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/ghuxtfzfq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gduzlhims.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gowacqqzw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmoovds.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gtoaylnsg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gybwxapua.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gydxgxzdu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfszkdute.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/grnczkxgv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gjdzjwokm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gprnrfldw.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gqrizezsv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gezeyfrwk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/glbglpyvz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gjgysbnyt.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/grvcogfsw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/grwpfqkgj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gxvvkaslt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gapinfaei.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/ggqvgjslx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggytxyfba.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gsbsivvts.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gxlummrmx.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gjbtyiktd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgobvtw.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gqsjfvqxg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gxvmiovir.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxgkiixug.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/glsqderfy.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gfshlfchh.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gptqvqrbo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghxziznyg.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gncewldwk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gqvhowyyr.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gdlmqboww.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gaqztyzvo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/geixevkdj.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gucuscxwj.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gcjyfohsd.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/geswdhpvd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gkbjzdhua.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/guggrdkpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqcjiuuhh.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gwrrlcghn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gqeddpefc.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gvhrxyjxv.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gvfqxjhmn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/glambdnzm.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/guvchefup.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gwwdhaudg.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjryczrqu.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gjdgbsnet.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gzdttndpx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gxkbnnuzi.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gsjaaucmi.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/giutgaloe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/ghykyqhku.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gfvnxywno.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxsnokuga.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gubqndugv.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gpepaaugo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gisucbtap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gfaxtesur.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gsiyawbof.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gjazaglkh.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gysalghyf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxvwwhzni.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/guogntfds.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/ggjrgkycq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnbpypsch.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gvkggwlnb.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gaqbtjico.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gycyiwdfq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gnhvtmgni.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gylwobalq.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gexbqrgec.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gmcqdiqpb.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/glhwgwxln.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gsehcsxhl.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gacdlrfow.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/grgbklxuw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtcmraelw.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gowzlgqol.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gctbwvnuu.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gqyjfklec.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gubhwmets.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gdvqehxpn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/ggiwhiaui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gwufsyeqe.sHtML


<!-- 参考信息 -->