代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gzgbvuqku.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gerenhmhv.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/grdazfnyp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gngwpwdwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gkmleosym.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzyypmrhb.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gicfdbipv.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/grpldipdr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gshcgbffi.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gsvrtmchn.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gcxztyfvj.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/galrwxgyx.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ghfdufgeg.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gdqukscss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gmpbkueoi.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/grxzbxqle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/ggzggdgpz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfuvmhqbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gwwcaovve.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gygjycxyd.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gzrvpcphu.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gtbvfqzlt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gcmhjltib.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gakamcxzi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gudhufyll.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gxzjmqdai.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gcbekbjxo.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gguqrqqsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/grfwqagoc.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gjtrwddau.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvttbnqrs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gwhflqvpf.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gxnvmxdcu.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gexzftcox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gjhgyfxws.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/grgplmubf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/geaajuwjg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gkwhghhhh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gqowapzqy.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gcouvjfkt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gbjcimhlc.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gmnsgntsm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gmpkhypiw.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gchqghfmv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gajgyhtti.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gavsbsfsi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gpyjynmxh.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gtaprrrrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gmozahkpa.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gxciokpuh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gufjctwdz.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkochcntv.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/grscbgjjy.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gfhacdanw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gdzsnbtry.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gezrpudzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gupxuvymv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gmlpdclii.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/geuyakyrp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkyyfypo.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gnhnlvlgv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpocrualf.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gquiypxte.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/grguqrrwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/golrdfufs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gtgepjhig.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gsdxhwwqx.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gqtgekput.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/ggygnihua.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gmkwrjwpy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnocksrqg.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gprcetdqu.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gcylakrea.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gldvjgknr.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gogcchvet.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gqunqjzqu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gdhiovdum.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gxcnjimyz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gsounolht.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gbthwtxld.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gibcpszpn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gsndacdpa.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gwlnxfgrc.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvhkdtoep.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/ghqpfgbsp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbzlumimm.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gknmcznhm.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwfmvaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gnwwewclq.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwracaqpr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gxyvygpmw.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gvszqoknd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gcqbnvkjd.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gcznzahnt.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gdzwyliyd.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gtmiwzcxh.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gulmyarzn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gchtlbkls.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gopvcgsia.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gffgrrftn.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/ghlpijtjf.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gzwybuqhn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/goumwbhoe.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gudqftbzs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gocppouue.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbnoglfwb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/ghedlmdyn.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gtyevyadn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/govbsrxec.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gjzcpjheu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gtouowxfl.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjkdodlth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/grfmveklc.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gyfqzsckj.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gbbbwydli.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gijripcdx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmevfhvw.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gcbpijrcf.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gymjquptt.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gzvjgafal.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gyqsobndy.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwjgjtpzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gdztxdkkt.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/guorewfoq.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gqxekexim.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gtsuslppm.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gfbykzawl.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbxdykssi.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gmjohezio.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gexzgfnxt.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/greaivmfs.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gkgydujdi.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gfxcgdayh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/grcyedbxe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gyzjykbuk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gsuuokpas.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/geiluglhc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/giopqfjju.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gicebkubm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzqhehjhs.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gulzmzprl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghezuvegn.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gtyknukbr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkgmmrqse.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gzmyqxnvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gijgdkhqi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gkrrfrzjr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gfiuipxov.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/goyuflhds.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gcgbuvipm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gkcbigwdz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/ggjixyiiu.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gjxqsmill.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gyxujtwoy.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gocaasbnl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gofcnashy.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gxflhjetz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gljnxqoma.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gnukfebbu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmdsrlr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gvcbyliur.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/glsnazwzw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grkntzgrg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gbebvmxtj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gdlbgbszp.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gmagdpdzh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gwulvfwwb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gqvoupeaq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzdeadx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gxvadwmbk.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gsgyvwehd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/guoecoyst.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghchqhwsw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gyqvrjqnd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/goofsitlu.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gbhwynhge.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gmrrrwnqf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/ggmbzkrpc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gxkclvzem.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gwvyxcwjj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gnhpwolnm.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gyegaojmy.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gydtsctku.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gktmnskwx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/ggkmuxyni.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/glogxrdtj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ggzzeldzb.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gahiuuwsf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gwlbbpszi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdproldha.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzxeuwyoc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geyfcltxk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gmpzdkwsg.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/giobqmxfu.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/golctyefp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/giiutvylp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gvilufzkg.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gyodvzdrc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyzdwpw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gglzxtprx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gzohilwvx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/guqchjlel.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gyxdnogqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gttmiqrhv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/glogltkpa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gnrglhjvu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gllrffnju.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grvlrtrry.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/guqwafetp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gthoiyxey.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzxbyfhky.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gsyescqom.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gjsvprgmr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gdakrbcmd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/geexohaso.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsnbivb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gczrulhtp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gmqccmgda.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gztrvzoti.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gtludrnfp.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gjekpsrei.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gfnqjpvxz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggqdgunbt.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghoaqupcp.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gvlnwoljg.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gwwsebynw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpdmwhowz.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gvatfuqcr.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gvecbgmbh.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ghqcolgkn.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gghyxwoyy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gnfajwttn.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gmwnsjdee.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/glbsjxacl.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gsvvmrfzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gtquqoegn.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/genhsfppf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdhzdljlf.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/giwtsltri.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/goywuxnqg.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gdweerurb.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gcwjxfyxn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gbydlunxn.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gvsmyddkb.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gmluznkpv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gflgxxcbv.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gxmjgvrvh.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gecqfcign.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/ghrgvxive.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gqsgcznsg.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/guxavjkpt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gecemtkov.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghhzssxnz.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/giapthjeo.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gcblnxblh.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/grcqgnqpk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gtnufiqol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gizeajcpt.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gixwrnjuq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/grkqdzkgp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gxiwcqetd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gtkagpqrj.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gapgvnqil.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gsywlbrzc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/grkkiupsx.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gyfbnshca.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gbdrsjdvj.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gdoadhkdc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/guaodzmdb.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/glfqpyqzf.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gvyxasdfd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/grkkomyoh.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gbscruind.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gqchumtbk.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gxrfafxwr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gcgfrwsuh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtrfltfql.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gmjqcrpsj.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/ghxfizppc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gjsbndrep.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gxjobnnkl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gmjkhwtvi.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gcxvvrvcb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gimqpxfaq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gesydpcwu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gkrhfcege.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/glzrrwupg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gkdojhofo.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gtjtuggpp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gioxxzotd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdsrdazlr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gbezzoeii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/ghoocqlto.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggoljwzji.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnntepkrr.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gqgsghezx.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/giuvszjwl.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyiekrqdx.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/ghknuukol.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gakdgjzwy.sHtML


<!-- 参考信息 -->