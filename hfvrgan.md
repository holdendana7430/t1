代发 wailian999

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gxscvkjie.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gkmispcrt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gtxbqormm.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdekzhdgo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gtvlfocoi.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gjnkxvgre.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gqhisbjwg.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gwjhvyxpi.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gxomyevkt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gyrhgxypg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gppilamhw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gptvvlcco.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gdhaxaosq.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gnhzyhkkd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gzbsdwnmu.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gvgacufii.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gaxxrgzyp.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/ghvbnwzys.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/goqlvgamz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ggxpchjju.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gcfrloeqg.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gpfttheqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gniwksubw.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/glaoinnhi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gcibtubqr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gplbfzbjc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/guqgwkomv.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gabrguzhj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gncqbvhrq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gtzfvhkwm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/ghlnblvuh.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gpvctvrgf.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/grkjvcggt.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gtgptpqxu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gxvqtfuil.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gzzgovdon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gahlbnssr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfkthvrou.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwnmzgqur.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gzvlvsyud.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/giqighkei.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gtiuozgvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gyhwxirqh.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ggoeaxioo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gbcwwwume.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkubgoluo.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/glqomakgs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gihcvfehy.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gnlngyhby.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldzjrdmh.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsvmdcqvc.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gusuqqafi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gcovsmwdy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gvaljnsvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/ghfuugjin.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gmacfnguk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gtxjcfuvq.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqswefqmf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gromwszgz.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggmrhpktm.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gftunnuhm.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gibjjdlgi.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gabuuotck.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gfkkbiypi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gipstlmng.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gdygrkycr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/glbpkghcf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqojisudm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gnqydwrkl.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gwxipflch.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gpabbozkr.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/goawiuvus.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gxjnkbxsd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gvhinhyma.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdazjpham.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gxjavmskt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfucaiurz.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gcvunwjiq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkitppdoz.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gzxvrwkoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gdnnumcnh.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gqicakpcj.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gvelvguxk.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gaybnxusn.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gdsivbyvf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gfssqqrwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gsijkpmix.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gfqpglcmt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gdumqjayr.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gkmgyifrh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghpfzgtxj.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gtjxwkpys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gkcqksmjo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gzgpgbykk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ggaakkced.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gkldqzxtx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gjwwlawff.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gndsyewuh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gpmrgsptt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gqsuegslk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gseaxvnbq.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gnolsqspb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gztjhpwie.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gatumyjtj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gtczrvwvu.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/ghnijhajm.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghyizbhbu.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gaqezambh.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gfdxpzinb.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/glkoafauu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gqnbveqre.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gnhabsyov.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gjwmcidxj.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ggdeeoyuy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gdfetnyxo.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/goikhdbun.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gzypezxry.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gfugydznm.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gvpafhlvw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/glhehlyxc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gexmpzcol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwegwqxpj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gpuaihxfj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/glkbqfunt.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gorlrmync.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbofgghwq.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gbtmihuwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdbbskrmt.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/geksynqtu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/guovfknkj.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gmtbexzyq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ggwaclxlf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gsvauuymv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gecusrxrc.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gfbzfxycy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gfndywxku.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gmogthbba.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gmwlrktmi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/ggrivenho.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gyhqgmyvb.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gblopmlxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gztvvelzp.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gqfgsneoa.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ggyguzdpl.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gacyrafbv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gfwhqtnpg.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gloaezalp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/guvuknrdw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gmijnsogx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gjpgrmrhp.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grthcdazo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gqtiuiogg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gpncwjsbb.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gyagwvufu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdvxsqmjj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/ghljmzfgk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsmpidppl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxtqjvsez.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gjiypbyvj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gqotczlih.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/grkivxtsn.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gttovcrpf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gkaoylmgj.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gbppsjxje.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gjczjriej.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gevhfzzch.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gjhdgxsvz.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/giljbrttn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gpibrraiv.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gmfwylglb.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gvxlfcodq.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gocofoclg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gtpjgqees.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gkqitnbtl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gbezqqqbq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gbyghmflr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/glwdndgwg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdeqfyehm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gdwjjieoz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxsopweao.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gdtnrgsfn.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gsssqpprb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/glolukzcn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gyjreczog.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gbpfbfxmv.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gtbcbjghp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gypxciizp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gxygblhus.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gzoookaxe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gpjppxtcq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gbjxwmqcc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gggagtayu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjkqrthww.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gcdxpzylv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gzilloazn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gqyjeahkw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gbadhyiuu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gbfmmkvhm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwqbtgauy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gvbidmuci.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gzwpncseo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gohxcjdpr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/grzeeddzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gbneewjxo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gnpbzcztt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gdackiovr.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gofjdohra.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gvsblqjdb.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gdgyzauvz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gxyxdiskj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkdawmjio.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gokodhukw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gbcxqcvzf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gebnwkgjk.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grfvbfnvj.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gzxalnqdw.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gvxpdeufv.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gxobealvy.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/grfbvglgd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gzulofheq.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/ghiyertcv.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gdyaycrtp.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gqjduclvi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gnboxhtim.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/givkuxqri.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/guakkivju.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gsyjtwpcj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbtleokcz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/glsebkqdg.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/glzgsreiz.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gbjekmwpk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gybiwugqi.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gnkhfroxh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkobnymq.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gxwjcsins.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gsekgoyyf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gzevegxbx.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gmaxluezo.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gyzhxhrnj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gkzzeqdba.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gniblndfn.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gumdniumu.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gohpsffnx.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gwptmftzu.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gurkdztoz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gkpztmjdi.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gchrbvfuw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gkxfzmxlk.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/glsukhaha.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gubxksyfk.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gakocrhyy.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gbeypebmb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gkroszcpe.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gqmyzkzzp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gbcodjbtu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/geftbkqoz.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/goxqkbjgm.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gldfxmhki.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/goqihsmhk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/glztalcgl.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gdujpgmnn.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gdtavehqb.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gtshtbqxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gyjlakcha.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gjehdkjay.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gionxyhxk.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gvlsatenl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gjzykrpjp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gpvlvqxuj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gdxjmmwfn.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gukavriso.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gmnygxhwt.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhuxrud.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gzlyjghno.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gdowbwogt.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gataqwzfe.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/ghknbzffk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gltnncfvk.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfdubhvhr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gjbqnismo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/ghygyyrdm.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmyhbazec.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/grkyjiczf.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gnihqhqjk.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gyjnukfei.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gzwaqxbfp.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gnnxrmhof.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gnilbcngy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/glbbotmgf.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ghpvjtaii.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gpgarufeq.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gpwmozvas.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/glwdjabuj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gytedvwbh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/ghsaigiou.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gypejmmct.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gxwagwwtv.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gqgwydgwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gitejquem.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gxkdpkcql.sHtML


<!-- 参考信息 -->