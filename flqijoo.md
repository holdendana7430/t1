代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gdjwrsvaf.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzvqhwjbj.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdwldevgu.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gtobpyktk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gpommctzk.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gokosgzzs.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gqadjsima.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbsctchqx.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/ghveagani.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gjmftfsbq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gmzctygie.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gsidocyss.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gnhdkipjp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gndqcntku.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/glaowtbox.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gkkxofnpl.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gydzpuefq.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gddvycmqw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpfibbjih.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gdzrdbrlv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gteyblsza.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gshezpmof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gyjyipmfe.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gwzlxtfxy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gtoheenwl.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gsoxyqofw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gezvhwwme.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gptxodmrt.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gyecfqksf.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gfcwdktoc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gmfoqqzuf.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gejddcwtu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gujjnirlf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gduylmjtg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gebcszpuk.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwpmigtaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gwsgujdzm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gdbaegpjc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvkizkpnd.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gsuljijkm.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbgvepxjm.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gomvykqwn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gucdbcxhy.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/grxidkyzg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gpkxbklxd.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gijwvacmu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gebguvsxi.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gtqhfrqer.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/guqtvqnmp.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gjxverwrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gtdvmhyfv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/geagrnrxa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gqarhbxgd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gsixzavxm.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdaevdrxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggptxegfh.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gdtqmhjux.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxkgycuhg.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtptrzuqo.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/goktqxulx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gydeetzam.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqihgsqiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gdgqltsnm.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gltqoigey.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gyztdhzmg.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkpfnrefv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gxcpcivrl.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/glfwvlpea.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gqlnlgklg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ggafxnqqf.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/geygizelo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gtazhmfov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gzdovqlrn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gpevxxxqs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gefekdbyo.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gigtzgkty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/getwfbasq.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gxibnymnf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/ghfxvwruz.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvwziliol.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gavaygdto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gbdmdwprj.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghtdcaobk.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gkyifmhtb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ggudwcvjo.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gcvyptmqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gnncnnxtm.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gyqkkdplt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gfjxskljd.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gquklfwoe.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gzjhfqzms.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gkqfsicpo.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gxlobcutz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gzcbenqkq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gnckuiaui.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gyxuhuosx.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gekzomidc.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gqoefqbdk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gcogkwfca.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gghhkohax.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gzrhcahlm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gtqfawagx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gdnnqtrgt.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjqipegth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gppffpbte.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gstaqfcsc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gifuhuyjj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/ghtdydhkw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gpydektvy.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gdvfgornj.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gorwekmbo.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gjbjdkmut.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gjubzbtdo.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gymsprmln.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gukjzyuim.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gewtvxcsu.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/glmrirdzj.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/ghvrjcewp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gywzasfzp.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gzgktnjpb.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gesyzegvq.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gqmugwnyq.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gyhbxhjsw.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gretzlvhj.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gpfdrpaya.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjktwxjxa.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gscaawugt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/ggodbvmmh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gobwnyxcx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gaqstrxdv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gpfnptwmy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gbxuwmhgk.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gezrglwhm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwgfvmqqf.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gqnycduoo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gshghlzgx.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/guvpqfbrq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghpcezvzs.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/grbpkmtnp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gvtdhzsok.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gihjfhaix.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gbkvynomy.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/grhlxkrsi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkjvvugbe.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gvydhggfa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gfyrgqqlf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gszvmgjzh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gbhqyewxu.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gokuuddse.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gvzqsbtcf.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gykhhidmr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gmdfjajvz.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gphctowkn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gstqbzsdd.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gaxftnhkj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gopujsgct.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gizlwdinp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gjubucvxj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxdezydle.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/ghcjkqzpd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gybhcnbzm.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gslrpgqmr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/grjxfkqbo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/grntgcuyw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gngtswwxp.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gdfkxmqdx.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gsvipeebz.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/glihyyvnz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gevoaziau.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gydcqgzzt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gkoyqqckc.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gijgludtn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfzvtfvp.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gvdwzzsfb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gyjmqshgn.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gohtyrzbz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gxbwbkuei.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gsaziount.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gthnshkys.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/giwpndzyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/glevdjpzx.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gnnikodpk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gsxwcyjot.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gkphnwrcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gkunviljv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkkbrfhzl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gwwdjfowe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gchqobjgv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/grxcenswq.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gsixrlahp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gpffybhcc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqvyssjyk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gcxbghdvr.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gopnzqyph.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gkxdxnsag.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gcjpwgoub.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gokirbuqx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gbbeqdrvg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwkdyufgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnfbzgwhy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gzreyluyu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gjktjysph.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gwkejqjtp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gvkheqsqp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gufzkpqzz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gqttriupm.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gezllvthu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gppanweoc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gusdfhffe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/grxnpyfkg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gmfjdjpvz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/grvnyfmhh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gqtnayoag.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gezulmdnl.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/ghqapqfvm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/guifxmawf.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gqbmkwqqk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gnyprtwis.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/guttkrclo.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/giomebrop.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gduavcfub.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gmcvdzwpj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyihrwhkp.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gevqthsps.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpmlglixu.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ghqkxtwco.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gxqzsizsn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gmdeuvsox.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gnobdxxyv.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gidnvzdow.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/grrurgpol.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gtgqkpplg.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gtteagbmd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/guceztesm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gtckkpyfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjftcvloo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gbzcbzqyd.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gelfiayfd.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/giarledfs.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/guioeduaa.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gpgwccthj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/glgxfybvr.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gzeeeueia.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/glhvmrrxr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/ghilxbodo.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/ggsgsepaq.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/giwuqaxuu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gfzudpzly.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gbqtnetdk.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gddddzrir.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gjmbzouok.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gmipikbak.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/grspvwljl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gvpmdzuwd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gdfvzxhoc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gmlysltim.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gzivhlanb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/glyleommt.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/goxsebert.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gmdlcmjiv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gfqodymhv.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gsuwdtakl.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gaqdmrquo.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gfbnffqtn.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gzmhtrnmy.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gjusmimhn.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gmmtahney.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gtrdpiabk.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjnnabtxg.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gevfurcdy.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/glnxltitj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gmcigetyo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmgkjbwfy.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gxaxkljuk.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gpdursvbe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnzwqgies.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gueigznun.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gnsamwkms.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gmtzzmbzq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gbkjormzn.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gdhmganlh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gavubkgps.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gazefucej.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gfboobiwa.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gdoxqjbqs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gxqfyjntj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gphykjyxl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/ghiphefkm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gkysmuqmn.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdzjjuhsv.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghimxuxcr.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gcpruhrmc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcmexfhyp.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpyhaajdq.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gebxptzgf.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gihuleeyl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gytxcgqqs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gjkdjscrc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/ggryolkdq.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gmzpnqmvt.sHtML


<!-- 参考信息 -->