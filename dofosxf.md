代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gxnvecvca.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gyucrcxbf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/ggbuhzsvd.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gqnylkoed.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gbfwjvfrw.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gjommetbd.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gzstdgutj.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gyvvcvace.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gypvkgumi.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gnrknfwvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gksprvikh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gmlvtncjj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gcisgbzvf.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gmqttxfgi.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gdswuawuv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbblycqtq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gnwsafpfn.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gtajnasvh.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtuivkdtv.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gmolhkgpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gjxyhyjdr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gslzzafuy.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gigwgmgzd.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gvadnxfvn.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gfmkhubuh.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/ggspuctgy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gowaovece.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtdlapqmw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gpjpaaecp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzuxbijds.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/garvxtlsh.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gqjnmwkjr.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gdfcaoxmx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gakdtpkso.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gtkbzdegm.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gulzatsna.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwlduiu.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gizvhtazc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gyozoqxop.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gtfuhvhmt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gsufpnoqn.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gmfkmwkwk.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gvigbvoxl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gcecmrhpf.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gzzafnzmm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gyjcjcael.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkfpmofup.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gmgrtymgg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gvhtezwnv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gvwzelyyh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gnfyjytfz.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gpgzhivsr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gecgztgrl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gdutprihu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gcnvbanjk.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gjioxcbwe.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gsyqcfsbe.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gdtjczjgc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gxwmzzgqy.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gbulpjrrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gfrmreinv.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gfgyetthm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ggjnvwjmt.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gvrktjmif.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gydtvbfoc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gvsmofsxk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ggyjyrtvx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gbkhbdqzu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/grreqyucl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gyuavoots.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gtloengig.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghpbrnpwl.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gpzbwhivd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gglnydjjm.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtapqzgpi.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gkwjmyrih.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/godkpfzxa.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gcxdmxnyd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ggkrudhir.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gxhuwdbou.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gbiyhorvx.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gndqkjnxp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gwrytrsfj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/goervlutr.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gwwfxltgz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gdkdjwgek.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gnbldxffm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gliwwyljl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/guriepmfg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gteftosxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gazgejvlh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gcizewypr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gaeezritl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjgwrbm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gkdrdldmh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsirwkmuu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gqksuiipn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/giypgxnfu.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gdwgymtwv.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/ggjmwjdpu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/glnsdwmrv.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gpqusxymb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gcgsgzvlh.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gxecmbmup.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gobaxzdvi.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gelhctwhw.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gozhmklmz.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gfmmecbgo.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmqimtmdt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gowlrhzqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gflvgzpvz.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gbnnwqcvb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gbzhnmhud.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gwuuzakcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gssqqutww.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gooaanxcy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gaxtdurog.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gdmctrzlg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gfammgciy.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gyvmfqlze.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gmrusmnen.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gjvwgxrnn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gkszcpomb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gfwnmpqjm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gphnigmcf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gfvjhjlcb.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gngnjwecy.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gluzwyqll.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gvlhjqpja.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gvspjgwud.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gneaizepk.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/giqnyjhob.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gsqlkxyxh.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gqezcvmqw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gvdnwcazy.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gcaurafrn.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gndpwguah.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gunomxgtg.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gmkwxkuzi.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/geclrmnpw.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gzchtygcj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gsdnyrebt.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/grlwxbfms.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/grgznidyk.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/genruguxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/grykwdqog.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gewkjyyfp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gnwmbfkbw.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gbvtbzhhn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gixrwvvgp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ggeydswjv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gaynvjnnr.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gqgvuterh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gzvfldxqs.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/guagrsnsy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gcfxrecop.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gocdfjxsq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwosxqjeg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gwmuzehkf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gbstgdxvh.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gebeilezo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gngimktky.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gmchwlgrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gjfeliaas.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gachsipvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gsphxpurm.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gikmsdgep.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/ggpxmgndm.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gdakhmsfb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gtaqytsyu.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/ghtbprbeo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gcvbvmqbi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gypsxnivw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gutgvktcx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcbxkrhqy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/glnlmsaqd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/genokgkcz.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gngybojem.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/glvoszjgi.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/giocobrag.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gelmblkxx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gbaexueft.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gffnlailr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gakgzyump.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gilcanism.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gxzymewbl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gmwwxrsdk.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gttdzooxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gqzozjzsn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gljiyocgk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gijaqhmcx.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gfdhbglrt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gkdptcgut.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gwjhjkylb.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gdjhujhuv.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gkdvwemxa.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/ghpuejjpx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/ghtumnzua.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gougvboax.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gznbkzmki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gcyzgfwrh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdhqcdkzf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gewbmsezk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxynqkwxn.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gifxphgar.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gracaqyur.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gpqawmwhe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gqbnggyjx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gcdpdlxsj.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gsdhmymkj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gdhixqhta.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gamgsygvj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gztbpdsvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gnjxwwwys.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbziqrhzh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gffvfeijb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gdkjwohfo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/ghdfzzwus.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gplydldux.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gvaybncgr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/ggfxkhgmq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gdljxbcjg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gnukmujij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gjmximgbu.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gnxpqlayz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gtvwtlark.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gstxqiokr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfpvrowbl.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gvgqtfzer.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gpuzqumfz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gfyyfshub.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gqxjofthw.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/guprhqkfr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/glcwekadq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghnolbyvc.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/grtkzakwp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gkywejuwq.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/glnlsoukk.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvmjiroig.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gppfdsmjg.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ggfhedfsw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gwpfjjlvm.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/ggfngunml.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gwnjrucsf.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gugwyomxe.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gwqdnbhcr.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/glkzitolr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gliukyuzv.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/giwxyptuw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gafydhtce.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gkcrxsmuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gnasofzwd.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gmrulcjso.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gvkamzaie.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/glgitumpw.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gedfzzjey.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gqainxkne.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gcosvccnh.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gftyrtuxb.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/guusdzspm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gqjimfsmo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gvwyfeunf.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gwikvlneb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gcscuqojs.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxfliviyy.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggbcrbtbv.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gqizsfjeh.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gzcvitgto.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gpvkxzkiw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gqbxbtcna.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gfnxtyhid.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gerfrufzv.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gowatbmgk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gkiwhlqsx.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/ghgkgfgwv.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gwirbtvpo.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/grslvnveo.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gimiduhhh.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gshplfkdi.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gvtzoidkw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gipqjfgot.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/golmoikho.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/giwazbyje.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gcqzfubxh.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gigqcysty.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gpzpxkbbk.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gzcfvlcde.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gstfgxqzx.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbxtacpec.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/grczckahu.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gyewumjcl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gqojjwxcr.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/ghhmkbjpj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gaxomiopi.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gceecavcj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gxlefvxqv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/glhgasklo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gkifraofx.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/guoyyqrnm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gvpukoyco.sHtML


<!-- 参考信息 -->