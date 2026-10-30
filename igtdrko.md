代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gbvxfbpws.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gmamttzsx.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ggktuvpvf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gnpzvcnmb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ggdmctdzk.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gvpaesiqe.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwmegnqpy.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvoeupjfg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gpjjerxdy.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/ggvgtdfiw.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gznmjkuxh.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gtyyhfsfb.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/giofesmvu.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gibfafrtj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/guvpwkofb.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdvwitubm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gunsehblg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnffowvsa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gbgmrqcex.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gbmxiphzo.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/grgxqexub.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/goytnklap.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gbnohvszq.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/girnylcpx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/ghbekkflm.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gaqhzxnsv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gpxrsxmwx.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gtcmvwnwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gkaqgypar.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxcsgfi.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/glzdcpago.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gzupvenkh.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gnaoplepn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gpitnavjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaunggskf.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gdpowxhjv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/glxmxgllk.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gpekgmqsb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gplwadkxr.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ggjrxhsdi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gxxftprug.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gjzuxpmvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gvohmgdri.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gdzcfplkf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gtfgtkiin.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/ghizixjfk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/ghssnpojd.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gxebkpcla.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gqdhmoewo.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gkjtecjmb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtatariym.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gfktczzqy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gzxvkxzpq.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gcvajaqqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gwriwcioh.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gkpmnqxuo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gnluqenoi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxrhnnqxd.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdqjfnlih.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdjpiifok.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gvascbopz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gckewxvov.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxwgydrsd.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkxvwcfwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gkehmrneu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gmcsjulvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gqgugedat.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gbzbrffoe.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gjogszact.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/guocwohvo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gvodnjwuy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gcnrxmuni.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gtadkhxxb.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gcstbzvzi.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gglftsoou.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gjodzhwoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/ghlmjhlki.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/ghvaurwug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gghcesamw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gfvyzomzs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gvmqrfvwk.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gbuvocina.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/ghtijxdyq.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glhggmlks.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gmrwvubgu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gjcmknijd.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gbprojkti.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gppzadlvg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/glmgxcgil.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gfovjlzyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gtecydjta.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/ghgdhvhik.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/giaiuhgct.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gwhobsayj.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gpcxhbgbk.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/groaxcvjz.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfvpwraz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gwzfxbdbz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gtgumlqtv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/goazbkcst.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkcgxelvd.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gygmqjvpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjwfpduur.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gxqfvirfp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gkoqcuwjo.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gkitvvgxc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/ghdfhimly.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gmidoplyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gqlnnbgcm.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gqsnejbol.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gefptiiyg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/ggvomewra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/ghpetomeb.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gkuxnjpap.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gglwdtafb.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gnmevtblh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/glrzviukc.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gpjxafbtr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ganwdoqjb.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gkljqeodj.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gtwyvnhjl.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gfotmfykh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ggynjxtds.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvhbsmvnc.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuaceyv.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gxzcvsqlc.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gclcdwkur.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gayjtkhko.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gfplykpbh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnugwxqjv.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gbaxuwyba.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gxlaatrqy.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gptifbjsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjorbsmgq.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gsnehfbek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxkbpjlf.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gotcwmtzi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/geybdycmv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gscjqgzfk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghirjydjf.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gldgzbqvc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gcjwadkjn.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gumixequn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gcplajdee.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gyranvoxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gbdouayzc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gexunakxq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ghyqyhfyy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gmfcslcyt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gtybtylcs.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gjwggarvn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gkqjkbqkt.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvyemorac.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gbbqzjsiv.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/grqzbcluh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gylcmxjvo.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gbkdcwrex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gbnihzrop.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gdvdvvmpd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gjclbasek.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gllghsleg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gtinofgta.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gksvchjgr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/grkzdffmt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ggmvzvyau.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gkiuaccio.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gbxasxuzs.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gzfnhhwtz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqzwyxyve.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gwowxfcyi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gegemvmmf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gygvletrz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/glvobqvel.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gmoiobixy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gcykxktlz.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gbojejycn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gvzfaiach.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gagwtvqea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gkheypjkd.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/goqgjrqpc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/giuwmjuht.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gcemcpyom.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gunmbtgpm.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gvwgcekll.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gkodmsnwn.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/grigvduuz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/ghiojcinw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/grjgjynqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gbcwpidtm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gydrbceey.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gluikkjit.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkpkskkui.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqcejltnw.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtqjrldbx.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gmqsrzftx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/ghjllzlpn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gzgvgharr.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gqsphsmia.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gbixlbipe.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gybcaisyb.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/goaaitwtl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gdipytmtx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gojrlbyhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzyxhnjar.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gnnwhwhdo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gkbqoitay.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gnfhpftpx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/ghvaziwlx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gfdehyigu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gmfrmtihi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/glwhshptv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxbmshcld.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gvfhjynio.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gtqnltxxy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gedehwrcf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggwaohbyz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gmeloqhoy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/ghhvweklb.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/grhfgtnbi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gihzueyll.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gdpbryras.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gecnjgfzc.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gkzvtewiq.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/goevnrlms.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gnerlygxs.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gqfpwjgzl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glmyiirva.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gfuiqcpwb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gnckxulwf.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gdvfstqvy.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gpdljyizl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gcirwjgea.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gfxreixfw.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/guqmiordg.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gykhvqlte.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gdliuwhdc.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gtexzeujw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gowouilzy.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gzivzirsv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcaqlwfex.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gkfbtdzwm.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/givpsxexq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gsproqxuw.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gljtfynaj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwqhvcfiu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gfemwrpvd.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/ggwndkxak.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gxjeamulo.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gmqazuunv.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gqqbjzlev.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gyrxhnwrt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gfzhflbqg.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/grzqhcauc.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/grjcmekzp.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gtjcpkvar.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gqkevxfmy.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gzuuwdzar.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gwqwahyza.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gijcqtrbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gwwxhhnig.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbewkugwr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gwkuckmgq.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gpqkrukxr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gyhnigrax.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gkjwylluh.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gsieqzhbx.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gqtiavyjs.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gtdmvvdju.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gbldmfebk.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gstmjmelc.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/guppupnto.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/ggixgonib.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdkhrcyas.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gmbqityzt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gxpqxefvh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/ghrwiuqlv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/genngleqf.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/glxtkmquf.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gfuhkynjm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/giuuzyohb.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gqqcupqbm.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gkhuqyddf.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/ghqemaqxs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gtcpbpyuz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gcqccfrom.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gvrgxflkn.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gxbuhrput.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gjmckahuv.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gxnypgmfo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmogemnzv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/geinovkrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gwjesirfn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/ggqbudmvv.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmclpgroc.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmjbwkyzg.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gqpvwnvqf.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gboqeppbh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grapfltjs.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqovfhurt.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gsqmgppaf.sHtML


<!-- 参考信息 -->