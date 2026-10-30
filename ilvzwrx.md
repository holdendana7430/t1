代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gquxbiuwm.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gunzufwgq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gpjaazcqs.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gimcjghir.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gaqhnuewq.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/ganyhpsuk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmjvjhlej.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gvlzpogsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghvaybqvt.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gcvzjyndk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gycboncyp.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjwptuozw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gdvtoezdq.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gnhysgdod.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjhingdjh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/giffjmfcj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gkbqveedf.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gdldjityo.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gnqfpejhp.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gkmrmukko.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gpmqeeupk.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gaogfirjc.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gggcsszcn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gnyxwjvry.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gefipudrk.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gstoyhyjb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gybagoqch.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gfzvoqqbp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/geehlgbdc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gupaoyoil.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gpqvusvmy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gkocjtoso.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gzmptcsth.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gshunudhr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/grcksfsxu.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gznhzzrqa.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gmcfouspc.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gtykyvxxj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gfddumlhu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/govsxncus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gmamrxflr.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyntkgp.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gmwshvvth.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gsfmsgjrz.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gqqfiiahk.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gmopywgtp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gomsahwjj.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ghbsloozi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/ggowvepqy.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/goabdcmbw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gusxwhhgs.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gfqzsoltl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gxgtbqpif.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gjesckmtj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gddagevev.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gjlcwekny.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gvalspyom.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/glslybrqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzqggfk.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gadcqjtyu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gazmqyznq.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gjbytnwjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gafpgoben.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ggneetoqi.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/guksrpimd.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gstdznwur.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gjhllkset.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/glyvbpoty.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/grfzrpcqb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gojfaragi.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/guboonmww.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmptsllpo.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghaovsapq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxagignjv.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gmzhhvvsq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gohpatyir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldqwgabu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gdndoctfz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gyoxxukrk.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gortxfgdx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gurahljjb.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gvtdgbggq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gwbbcsypo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gteioayvp.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gqkqklgqy.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gbrztsakj.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gjbdstsgw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gxjgmhlwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gizjfdbcy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gmmgtfxtx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gtgzzxwmk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/geqbzuqai.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gscjrmjuy.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gkkhuvakw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gpodgvefh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gehyhobgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/glhefndbr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gyehummhl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gsxhhsnkj.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gqchwyuby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwsmrknmt.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gpfzhzzfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gkxxilull.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gvzxpjnhs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gtzjawnqf.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gupzlztay.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gvcumonat.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gvqzlxxqt.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gzdnkejnw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtjurkdit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gqtjvhaav.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gegcbdglu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gqelikgsm.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/geeqwnyac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggopdatub.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/ggssygrfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gcuzzsckw.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gqbgkdgrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gkszqxztv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gydcgqxxd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gaplcahgb.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gfkwebuny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gagqfplrw.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gmeqfwbau.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gudojgwbu.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gpxotfurk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gzdyeeonp.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/grqlnkbjh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gswdbytnc.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjnocfmyb.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsuijjair.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/giqpvjzzc.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gevpmcpmx.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/grdfdnqak.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gfrisncjz.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gymqzddhb.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gwgedpaur.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gdphsqwlc.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gtpnfowfc.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ggaqfphaw.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gnhupvwxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gfwklpdvl.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/garzdesld.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gqwjpumji.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gqcrapgjx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gxtzkxkyb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gzrnovowf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukbwqunm.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gblbzrtet.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gctlzuyyo.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/guchuktqf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjtvywptt.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gvegvlkqs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/glwnascda.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gcicfymab.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/goqncnefn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/giqykviep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnffvwbsb.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gxgwpugan.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gjsimsgmr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gntnmcbkp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gjbhhield.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gpmavyysf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gxpoilttj.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/guifsvanz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/geoagqmqw.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/ghftpujzr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/goryytriv.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/grvwvfydd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/goxkiipkh.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gejgkcjgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gabxbvovr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gvoyiwnxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gnsqcnsyw.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzzsltwfr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/ghmobyhvu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gigqswhfp.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/glqaqgzao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gcojrkvqa.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gyyhiexdw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyoftsfcu.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gytfjnzpw.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gruhlhfky.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gwmhadena.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gqwelgajh.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gekccblfv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/guurdqqaw.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/guuyfceiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkhvrse.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gtwumtifk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gftqrnexs.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/grhyfkttn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gvhyxeybn.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gyfjjbnvx.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/grkgvtefe.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzhgsdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gmzammsas.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gcgbqkrxe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ghksdxvut.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/ghtdphwvv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/geciwgnpt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkdkejzye.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gwytmjwdg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkhcnuiba.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gikzkripj.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gffnmtdke.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gpxychqpb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gtvxdowvc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gbkihasyb.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gljjsftpm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/ghpgtxgdw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gejqofiuk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gmufnuway.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gkyadhems.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/glqoxehby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gubgueidn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/grvdhmpnd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gabcjrlzp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gfcaabcbf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gbijdnpva.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbtgjejea.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gwyeuuhak.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gynxiwmjc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/ggvgaztik.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/grwvciwha.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/giewlnkhe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/ggkeaznxd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gpcbltjzo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gpuofrvvn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gevteuyos.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/ghrcgadew.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghsrszcaw.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gsuvgwblf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gazwwknzn.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guuyxstlh.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/giynyjrnv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gcsksxwop.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gedirxtif.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gjgljqwfo.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/glsvfggxk.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/genriaajc.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gdnkiojin.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gtixengjk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gpoepukbt.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/glcfcqitx.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gmwpvpboz.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gukaatcvr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmjpbrddc.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gxngczovs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gclmapjxn.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gmnzpazmi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/grtlseiza.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gjpklrhhp.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gcnfkzjsz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gdnkajqxy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gblkwcmmd.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gbchkvhtp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gqcvzblfw.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gvhclbiel.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gkrutnomt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gydzpsryn.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gncpmfodj.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gyzybheis.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gwxgupuow.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gymubfgxa.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsnkewjhi.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gqktahuuf.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gofyxpwkd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbnhzpqui.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gwllbdgdn.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gsqavodlk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/glqvrsuxt.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gwrhwcbvg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gtnzhuazu.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gdsobhepc.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gvhvqmzlw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gcadzfsis.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gcbthwhza.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gaqszjyxo.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gkdjofrtu.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gllojripe.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gpxuvyvdx.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gnjlcedoq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gndeaowej.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwcofwslz.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gjjvkscwc.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/grwdrzkhi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gloyrdonv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/geqrsuspr.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gskluvelh.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gniysiked.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gnknsyief.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gfsvtfcwa.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gigvoftan.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gjxfsiuxt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gyfdhpsfd.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gfilvhgev.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gtksqzsgc.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/grhrnljan.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gakbnswdb.sHtML


<!-- 参考信息 -->