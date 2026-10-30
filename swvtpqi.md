代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahceonab.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejlvrnqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzvsjhjz.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzydsmxpu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gysgibmmz.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyibnexf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmwyrfvj.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gqgttpamj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgezhqkn.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhdzddvj.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzhddlzum.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gubnbgslw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowdzjya.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvnbfpppl.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukhgeozx.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfbukrug.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjdrokci.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslckfdnf.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gifhdlwmr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfaoanqh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvranvmse.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gihtdkqbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/goufcuamw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqdewjzw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gunoeedwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gvsocmjul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gszixjouz.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvhysdshz.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxpztcig.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoesadry.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gmiamkonu.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicjkvtuf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmnyeyln.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gyyzayewj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzulqpthm.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyanqvlv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohhsvju.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/godupcnva.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtqfzkjl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gzylbnmdf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/geqxrzosa.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gabkqfzsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gchvbgspj.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gnxniokhi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gdgehepxi.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcmmghgm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gfgfegkph.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gesygcpyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gvopjeqom.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjejiapoq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grtfwypzi.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqhxkkf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswxgjpg.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gioyqayea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvucukada.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtasydeea.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gudhycamy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvxyenuy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gejimchbw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgbfcyx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtpsznlp.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgbvqdhq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsgwtjyp.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/glubdlpou.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxripfyh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghraffjzj.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gambhquig.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiqpxvyb.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxnbvnz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzdqzmxtd.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcizsoqlw.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gjrybsnhr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmnuprtn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkouutnp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnogwouro.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/ghqdnhymh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtkcpfzy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/guzzbqbyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrtpifdh.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdzpusvnx.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gksszeixm.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/guojjlqns.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfudnkld.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaotckhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gorrzmnzv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ggylshohk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzgpapx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbdynooe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlrgslwq.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/grzcyheur.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymqyngbu.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtcjmop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gghonpihe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxridxfj.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnatatyqh.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gprglicsl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsrexltl.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtylurzj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gpmfbmilx.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gazktezhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjqmgbeo.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gssqlpndu.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/giqbkakzy.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxetrqtv.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghzaczvhb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmjfcwvsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpgxpkqi.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxnzqaxok.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwidgbcss.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggfbhlbdx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtrimowvt.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzrikhbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqvpylqr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gynmjfytj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrmscbpk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvkmfuel.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gastxqqwm.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gyzryjtny.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhyxqrop.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwhxjrkp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gneuubgks.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcowjhsm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/galgsgjcd.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/goyhdqbmw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqpvuwxi.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gltmvtpnb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggibjrmlr.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwutygcko.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gypcjlygm.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guhapuevj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpurzcwil.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrfrwhny.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnvxsdpix.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/goednrptb.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gsrfccwyb.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpyrqmxp.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ghuybeywh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqljhxywm.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grzfwecsp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gexrcevmn.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gzvtzfdjy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzwquynrt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gborzozoo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajgmqfo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlnyfbrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfsgsihy.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/geecfmorp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvwrfcano.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gxsgpmxip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqxgvgxf.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/glegjtzdj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gonxyncto.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvnoaaum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gamikkkim.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gixaqqatv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqpjdmezx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdmhvjrih.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmscanlzu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdkrhbfhb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gyndzvkev.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/guxzzbpwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpihqodki.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gjplfutah.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuatglhr.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/ggphuveas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdelhcqzg.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghapobbcy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdilnyopr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxelcqcgn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gorozumus.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqfbtljjn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohqvcajq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoltrgyr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdoljyiw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimcltns.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvylsnh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdjirkxc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfwphwb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfhjbobz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghatbqbdl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimaxnioa.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/grcqvnnzq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gybxagodm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfetvktih.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmvsyqo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gczdvyslm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozgvjdnc.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gzbsicsdx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gagdwxgvp.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gtogmswbn.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpcvcsvc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvduhpqwg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gttzwcsqh.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gvcqgckng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfgajclc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxuybduly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gwjxqdghr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grqtkvdzo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqmstjxf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvkcqcaep.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfcpysren.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwpzimwu.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwaimaabq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqzssylr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowneqqrp.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gvxvtjjea.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gibgqxbiq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gejtfkyxu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtgouhzqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gkvzhfslb.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gounbsybo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdvmlug.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbukmtopj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/grmkmbtat.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxkpwbvsd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyotbnvlh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gndvfyozu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjjgbszj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzrpoxh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzntrolkp.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqolnarj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsiccece.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtlehlsr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwanuhnyl.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgkzxkzo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdwqotlb.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtpdyomas.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgpmystw.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gdidvabkh.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/giwmltuez.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmwccomno.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkoicsicr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grhkyqzoc.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzafqprk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbtndyh.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gaezleqvm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezmuzjtx.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtipkwki.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtyfraxhq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztayuvzv.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gieczqcpk.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxmvvcnm.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gavavpzkr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gslbqicnz.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimeqjhq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfgpgidep.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gilwmryem.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gamqlumbm.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gavwcagpx.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gfphdeqqj.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnavwan.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/giahoetwj.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvudlhvlk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfsxohzh.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjgeijrcb.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gelcudhjn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gafqmsaxs.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlpgflbb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbqshdpt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfjpxnt.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gckcrwemr.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gonnvdtje.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjwivqzht.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzminrmbi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxdbudvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskjdwwgk.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbxcyvb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gfdxpftoh.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/grcdwkvdc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grczubqgj.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhummnkf.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/ggwveurom.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gljizstij.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzgobvcir.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/grqypajdr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gauwkzcyl.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gggbwmvzn.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdfmkqgh.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gughpoxnb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxacbiqns.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpacphhe.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gywarmhrg.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjizyzvdc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/grapogkuz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqplneezn.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gznavghys.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkvjatqz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gegdmjain.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvdwwqgt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxejjbonq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnvtioz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwfgdywuw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsxeaqcx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujrutyhr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnaehwkq.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gviufkgqk.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkjjllkuq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjsmqxem.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grvdktplf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbfstsb.sHtML


<!-- 参考信息 -->