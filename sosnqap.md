代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkwomfna.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbkztoy.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glywnfnta.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktmnkwk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmpndssk.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gooxxqwxu.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbqloczrz.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcajbeer.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geioauxvq.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxdqegfr.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gmmpqwcoo.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/geopfhlbo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzbekcxs.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxlfmezo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gdbxrexhu.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhpmzwej.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ggsigloyx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghoejbdvg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqburizg.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdzbovckv.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofcbvuhi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujujnrm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhkpsfw.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvcdxwhv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvnwutzm.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gltrjjsvv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlxznxot.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggykulbem.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjannntx.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwbirbstp.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyermlxy.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnedfwkgt.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagwtmgc.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gtkcqhkex.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwllhsm.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpwnzgbp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqycmgn.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gtvtzkpnd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ghahawtsr.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/goslnowgn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqocfyfl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzuicshs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/guamsscmo.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjogwheoh.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzjxwiz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gmcmcisfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnoghrrnh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpvsccdie.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gboqzylbk.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gepawrdoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gpedgjwkw.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkoykmgm.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gslgvalwr.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpqsvvuca.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmojdoxap.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqnouzn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqpcdpaj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/glnuaxfsi.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwftnwo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtmxdul.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galdfpqpj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbbhvqtc.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnhfncpys.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbudrdpg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/grkiwhbnr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gpzhcgtfc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/githpznbi.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftmhvixi.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gixbmthkq.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gsahfkbcp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gavaqrssp.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/giggukzhz.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gephmotrz.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghathvxke.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gfgldwpgl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gmuxucpac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnigbgdwi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdbkjzta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/guqwsxyrd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/geifhbtnm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywdpmjj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/goydqnjim.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthhujbif.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grjflzlxz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/givqjekmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzdgqcij.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggpawbxou.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsjuzinou.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzkbtgyo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ganfzueof.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjoopmmf.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfxuveef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghguthfib.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/geautpkmd.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkoaytyg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooqsipdv.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvmxbgckp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnaezvff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwrrgjzq.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gibxacers.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyxdeqys.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgisaxum.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvmivjq.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaifratc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtrurrei.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gvajmmkaj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmjqpmtr.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbqifkfhb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/glwlntoge.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ghxzzfsrq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxguznziy.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/ghyfofpmr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gbtttnrcq.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjiawpcez.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrcbpys.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkbjlmwt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glljgmxgk.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpnszzmv.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaifymbh.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtpafllpu.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxngxhgt.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/giepazill.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbzlbork.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddbgdqrb.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gujttnznm.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfaesvw.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqqjdxlb.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnplylotp.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhfuqdx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmtuoroj.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkhnchbyx.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gaszunxww.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/glpcvdzhp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdyrvouzz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajodxzgu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guilpossa.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ghcwjbcwj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvwavuco.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gqpreozsg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grykwfvic.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gzkxijjbx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgpalvij.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghtpoezey.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gnbjyzexm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxardmpj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuitqwui.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorlqevmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzlmozpx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegrfcvm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gbjuzofhl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gttdlzzcs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmvkkgrz.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewbjflln.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ghllidsfl.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjolldykg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyxwzokm.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlgwhvcm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gajdtgpqx.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gfufakxbh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzmctdd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpftayhuh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahhoyam.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoolimpd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gicikaalr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhypsumf.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuthboji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtvzmpy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhmdtfm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbfcwtoo.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghpgzvdmu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gugkdzwpf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxkmhgdv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gegvkvaed.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmurqlatc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/groqlxzsl.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfclrds.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnlewjavo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggznusgtx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/grwmsbhsb.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginnggpsq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdgeshre.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpljndeyo.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavbvtwbl.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmceqcd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxlixrsh.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gihqcptaj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/grlngmofr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfwnioqn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grcumkhdq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goqzsvqer.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpuzrpoa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrdjkrls.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjbxvocrl.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbcahfrvh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbyptrgq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gzfctzwdx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhucyuxc.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godhvteso.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gejngyxtr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswzqzaht.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwbgqrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbrkvoub.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gwcxyfpde.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gmzqwklhr.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrkwdeeq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbregmlvt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvksoqa.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvociek.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbjkhaqiz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gevepiugt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsacxgmf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/glyblcmgh.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/grocezxkl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapnwvqfg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkvmhmkd.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbqkhhn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaqbsxmv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprckmpo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdajpaz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzatazsf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvnugfmc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxtbebttt.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glylzraxg.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqfzzzmt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfemgruj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyrypgnk.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggjvappmq.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocwbqgst.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbcaaxbk.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gagtujzpn.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glngxxwqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gslhcohsh.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyoarust.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkslmhmki.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gejrlmxym.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsukqnve.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfyvxehab.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gootqogrs.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzfvfiy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbumlmriz.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gcoboqkaj.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/grbpwjbqd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/grgrjspfv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuzkdvpo.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/ghsymobko.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvshlvjyv.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfnogtfa.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gbqkibgzy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gujzsopmi.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxoztcxv.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ghuzbkspy.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/glyzdbldz.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwlfxrqkm.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfnfowzi.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyytwpk.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsrmefzkw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsxjmzgx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrhyjeyk.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtuywvrb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqsryeof.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gifyaouso.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggzswtokm.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glqwvtbui.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjjcvlo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghmlzkedw.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gevkowafd.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqrpmykz.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuyatxym.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzxwsmmsm.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpryufir.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswpqgzmv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gzjdatatb.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gupfeoafy.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gaaeuzpzb.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gkzdylusp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnidvnmb.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmakmidum.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/grcgcmrza.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/guovvceur.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcyibiwb.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxwracvbv.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkepqalgu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gizntpzgk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhrivemv.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gnskynblg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifaznjzr.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdojwkas.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzvrjtni.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/grimaigvg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwuxrxwu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvlwcik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjujpcsp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnrcojwej.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gotpejdsb.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjmcboizz.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjtodzp.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddxnoodh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhcdapjt.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmjayyuq.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/grwxlszjl.sHtML


<!-- 参考信息 -->