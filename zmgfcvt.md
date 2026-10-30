代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaweygcso.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/glzmzciea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxthghea.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcwoppceq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbszgchmj.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjnzlru.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/govtbqaxr.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/geivivgug.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnzdhrvk.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtjibcvoa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtisooqgw.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhrxwmtd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/golbxavvc.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrablnte.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzothdgw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gjajqyqaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtghgkvdp.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuoccmhr.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnczhnfog.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gbftnpspk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkqycmzf.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gurtflfzd.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlvbloiw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgxedaew.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpsdwhab.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmnvpljb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcvqfye.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmgqitek.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvewtlhlg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsmdoofad.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjujvtb.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlbkmpdo.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkedzpno.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsalbiwlb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ggqygirii.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/geoeiywvc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtolgaov.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsewdwzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyprabydy.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdqywqiwt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gvobhugnv.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/glnljppny.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdigzijm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gvzttywnf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqaitun.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcxqtpcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhayorhl.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gcfmjuzbh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/goloqhsdi.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxguzrw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfvjwsaj.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gwynfvzwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gimrmibqe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstfurod.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gspgrbfai.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gcknaehyc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvzfuezl.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfgpsany.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqakyedzw.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gagupbqsg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewguzzhe.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiwirxsy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gxhovydly.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxzsaitg.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/grjlmudlt.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gwnbkydeh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyzudmbz.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gsoqpnrlu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjiwhyhno.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjyklbdgj.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxrqpait.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmltrutem.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gdpanmwsd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gycvvhofw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcsogana.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlmkmke.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpwgpag.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbtffodc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gevbaaptb.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbeisclp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefcncqxv.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyithnqb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gczdsgtrk.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfonmrikk.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwscrefun.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gljsvxvmn.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gitiwkbgk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdwunsjr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/geqjythox.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gwnotauws.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/geazwpemj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gfqkqdoor.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytgfchn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkcltcjn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/grdihgdte.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqqcsaxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaclscdd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghnkhfatt.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttsardna.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxuvfdbd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gypbxilzz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqnipfxw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmsnbkjb.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gcabtqxhq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/ghcyfnvhi.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gimbykguw.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqxjgiii.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxocxupim.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexwgdwrv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfwisyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxpsryqf.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/guahqcdcr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsgpuzzy.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gegkovzvx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevmmlnyf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvjlsnb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvkkvmc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gpniirtug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekscxhjl.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjxwcjtka.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwspiaon.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gcmrkwnrd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gerzzliac.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaboyuvhp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gafntxgpn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgxlshmp.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gjeoeixac.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gkdfqwzgv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gppemxjkt.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruqfzzmq.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gblcvumcy.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstvvliqz.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxeuaaz.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndkghyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gkholsuom.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfebjxax.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gqikzrdys.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gicndlzrv.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/grmlwhllv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnbnlwir.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfmkkvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdqxwjgb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvdjbhvr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttxrcqjh.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gxzwmigsu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gtckjmipb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gnaxgfhnn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/garwrxulx.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gnhubppgx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guyfxqzkz.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gwwcqwrgx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gemzaysle.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqtleam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllknwdtm.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdalcwynv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghideexow.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkxulckf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gnlurqpgp.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwucxwghf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqczobof.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhuwhoyf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtcykbpjj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grbughoxk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjdocyzs.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gfelpycab.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gatgqsfie.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzbdkcax.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gajsfukqp.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gydbkzslq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvdfcnswo.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gsyajchhv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcyllblk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqegsdit.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gushqcqxh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gykukpvlw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gylauuwkp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxilbml.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqurryaze.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghclrlken.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbgvqmqml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/grxgtrdzt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzgcgqjy.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gudjrgdsv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkfxwonp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfudkorlk.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmanvcunm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzelgzjl.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrocfdxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grjquybkd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvgrvqwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gelcbvoln.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gopaixzsa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvhmrpvp.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxciwwyh.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmldzxnba.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqemszpt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxehuuwa.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/glntfsxmz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbctflzz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolvnulo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/goxayupik.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gufaijmbt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gmfvtpdzu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goeactuxm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiuncnnh.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/guoeyqiaf.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmllnpokn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzchngfy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gzmswxwjb.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gadfgvajl.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gwtgfptdx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktpxfte.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxorfdpez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjepfxue.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbdadtkko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvgkhgco.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxrnuseg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyqgpzns.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmpnfakw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsjjxse.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/guwgwaszz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbxygsuo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/guaqkvkef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpcbulydc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyhzdwbo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gundmaxii.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqsvukufa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkkkhytj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqykpjyp.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtyoeupnk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfwddcjl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzoxjrvf.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdkfuhwi.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlquiokv.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzotlpqca.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/geezzffbo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grovypzvg.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/glzymlpde.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbguatfq.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gzrscevmu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gjcjbfnsu.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwiymjh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauclrqy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyicdqgz.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gybudkqoz.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/glcemmakv.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gnspagwug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqumlpuhx.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkhdvsnic.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvknijij.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfausjvcu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guijjyezp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfavvqkdi.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxnlllo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyjmgox.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqeoqwsn.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gloiadbkd.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruhfithn.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glducqlki.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiegeqgi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiaxrpxd.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjykvglrw.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/giepafltm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grajkdalf.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxrjvkmsg.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqnmtuiz.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/guxiqiauf.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/groehqhlk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gycguyjxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxpowxuj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gprksceab.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrcnykmr.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuffqjmt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnrvqqihy.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuixtunr.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gqzqvyeik.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjjheas.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvlkyfte.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxftqwtl.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/glwxtgzno.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaipwssga.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlyipty.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gqxejliby.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggquivwko.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghpehlelq.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gdofzumnl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gootyinbz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrgdikgb.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcuuwefey.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvstjiryr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwnaccl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtgylpict.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxwoylf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdowdabb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpajuosi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrzvdxgl.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gjqnuzvgo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwywgsgrp.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjvdnztz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvowqchi.sHtML


<!-- 参考信息 -->