代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnmwwuva.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gigafkjyk.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvynbkf.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgxeirrz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjeezviu.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gztwbkeyl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaykvqvbz.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gztmliybp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ghuvvkfeq.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gxhxrkbbu.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjadbrl.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gzhvwases.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvmcphpq.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkvuinsqq.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gletsfpok.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/goxwtjsry.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouqejpne.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfyzukogy.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqbngwkl.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxefckfq.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gssktkgjx.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvowdxtm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogfuhele.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxykovie.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytnjqkhg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqwnegje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpeiguip.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvgajkcv.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrefqgd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpybytsa.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcxbfbma.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gndldnvra.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrftjikz.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/greswbray.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwuwugiv.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gupqfnvdo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gttmcjnhy.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhdwbonr.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbojdzehe.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gsbjtqbcs.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/guzxtzpvb.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gflucrzqo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfwvmiwfb.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gagadmjeu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwbykpaw.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gdudkznef.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/glvffodgj.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxljkjxhv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppjzqsuu.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqapdoqc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmbllctj.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/grdzcnroa.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gbfxrhyhh.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gehuojfgm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gupoehrge.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gafyxdiaa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsguyirxh.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvywfenwu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gykiyjxga.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgocgizk.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfpnwqk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxexzsdqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gobsiqpvv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppkfbbkx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gaovwpkih.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/grpjcalma.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/giwmfaopy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfnefgrp.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuvfvjoc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvxklbhrn.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grmoiupwc.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcfbkmru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbuntepi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdplhkvew.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvukxzk.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdebfohxk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gitszfqna.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gtxepizyr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gxyiewgts.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsfunmfik.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmpfcicp.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gshiwwzeo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsxahtoi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gieyjtcfl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/goznkotde.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/ghbwewonl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gzavsxwur.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gmibqqqad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijlzdyn.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/geqteppha.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gchgquqzk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfxhnnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/giaviczlx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gppcglbfo.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpqwpaong.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gffgbmpen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtajoqlgu.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/geximoqhs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gsjltjzob.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glonjkpbg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbdjlww.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwyfltwqe.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuocecb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnssyaeic.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glehmamiv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvaymoixb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrtsslcr.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxhvefnz.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gagotjxnv.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goiugzlzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gmmbljeky.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gknrmwtyx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gauwklrvo.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjdnapkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqyaowfe.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gubmiuxzg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/govjqhynh.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtxwefb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacrwtmfm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwexyldyv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrvwqswe.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteovaiuo.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gtznjbjzg.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkviifcj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcskipxie.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhyuklcs.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczzhuygh.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gikohehth.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gyguqvzof.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gczshhlnd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykjhvot.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/glwzksygq.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmbkgaby.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gazrblkml.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/goaxvwduv.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grqsqdchb.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvlexvmo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaomhelqo.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gddmvauwq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmdfrud.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxhpgalc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxitzdwk.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gfxowcmch.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gttqtnawm.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchsvntp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxxjiyy.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gydhgrpsx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxtjasac.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfozkuwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonoktbjg.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozknemy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ghntnbcuj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzvhjjvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gcourvvus.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gtgdcduag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gogdkuehc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghcywbfrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfukvzzc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdrdjjdur.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gltecceau.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gzwqytdif.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqwnhwpn.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrissuph.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjigqauk.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqggwcgg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuuqvhyl.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtxpeoyl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabzguke.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gafneeqii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrchlbon.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmympdor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwzgsuvy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcejtelyk.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmkaljhde.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gibrkjxzs.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gzrhrwnyl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gemvxmxea.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqrduetc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniajykhg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicygeqqf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/grycqflmq.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gsakgsntl.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gewbpehws.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gopqgyyaz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkjnvvbs.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gznkijjzs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnpkwso.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gugtpuwdj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gleegjucw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbyxkctg.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbtdtxhq.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gayghtgvt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnzdevxu.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmioffray.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gkbijhioo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqdqchojt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/guxzekkrk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwtxzdig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqlwxxzj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxkbfalws.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyymuixu.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpynjppfi.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gphlhqpos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvugzerr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrqtoatj.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/goleovggd.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/goibsjjax.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgbwiei.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gchguynds.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkktlkwa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjglbwus.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmbgpnwh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gepuooufg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsalsoegh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gyscptbrh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgbncod.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gotuqoqvm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrxaouka.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/guenbgliu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gaxyjjhoq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhzibhkc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gilqkudip.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkruzxewm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqfmhdcj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghcmdmxky.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhrugiyx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhskpgig.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gtkziezyp.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbkpdpc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdqwtnqja.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqowhsv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcdgdfyij.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxciyjjjq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljaauxd.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/geoxvantr.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/guqiczlnw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gviuclxvr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupszgbto.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyfdimhgo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucxrrkbj.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grynlmupd.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqeqdks.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gumovpswp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsafwveu.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glnpsedzs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbsiydcop.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gmzcdjgdj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwoevlfqe.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpilukf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnedrlqw.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtgddycn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbljrvxcg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbjxvsnt.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gritmiyfp.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gydckiaal.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghshroaah.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzutmcwt.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsfzorgl.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gzspypepz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrgdouvt.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gznjxuyzl.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbswtzzf.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtuaijlc.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlcfrgtr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxswgvsv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gokrzfcod.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkptzybvk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gstfowgwu.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gtqsabeim.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grysjkhga.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawlqnzfs.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gxbulyvfr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gfigaxpka.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfrvdlaiv.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnscdsze.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gkneijapz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gasdyqoty.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gbyscjanc.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gimmxpoue.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggngoetlr.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfijdgpcw.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgagkuya.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnpconygn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvgkljvv.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gouqpenzj.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gnktqdofx.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gicsnlcer.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiuiwkcu.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnoukiiik.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhlkdlrv.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxqatrfax.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewavacpy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gcppqxotw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzahnbea.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gyqpxipkc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/grshtlbzu.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/givramvlk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gznpaxdcx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwdxqwuvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gxsgyfwvy.sHtML


<!-- 参考信息 -->