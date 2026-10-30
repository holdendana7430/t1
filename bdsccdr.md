代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmbgobnh.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/grbeadwep.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwllkxqtk.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaoiskuc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeajbcqs.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtccnjcnu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbngnqegl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxpsxnen.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmwbobf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gorncgpja.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfayqlsk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ggswxtzub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdauegky.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gutvvzukt.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbbasef.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gxxqdzplb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gtphvxrcn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejufnvhm.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqkafgmf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoyophbk.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpqotrs.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/godnloxzx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwlpfgpl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genrvbpjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowzeztfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifqpvmu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gnlouloye.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotexxeip.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrqgthkq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrzwems.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gxllldqsu.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gukpjgdye.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gfqisjbmn.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpztdwsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goukrtrtm.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/ghuoohiko.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gejvkhqol.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gctopdwdv.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoqodqqn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gkcenbory.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbnstcwc.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gqywnnkou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjtzdytdc.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gqsujlfwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnpazhb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggymjwybu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/glqbjppdo.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdocdqgqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gsvkkxopo.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfybhvqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzegadwkp.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqgrvtsj.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkctzku.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/giqbmfiew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcylowftk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyzpujsb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtmwitky.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gepzmbnrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuhrfadp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfrdegyw.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gziedxuyt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghytvqwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/glcyckjix.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/goolswcmf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggqlzamru.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgfsbkpa.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrgvmql.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvxrzitjn.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsmoqkes.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxvteevs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlfvkozv.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/giiasskvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gabvqirsd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glrpxgjsd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzcejssw.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzsdsiqi.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gktemtbcd.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gelhnyidy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzljdporw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmlsrvg.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsldiweu.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxwckqc.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gzxcywhef.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggqxuwpih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaztttmm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvhqtggc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghoqsvjyd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkpakubr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsvneugzy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqcdvcnb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayawjzkh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilmzrldv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhqhwepe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaipddazn.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltnmitpy.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkluvzclb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gceswdpie.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghentjtqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwiiptfa.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqdocvzjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gewfddgps.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gasfmzzdw.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gnpwfsqrq.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gmonfnemc.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkexnahm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqfznvegu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gmtiklwff.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gazenvygt.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhblgvnc.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdyriivx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxracmrey.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/grzrvfeol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gtrykhrxp.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gblxrulzo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkvdjxeh.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gootprtgv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydzumgp.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gasaorupz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsddpfqxf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gzhfufmla.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrgawhao.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvuvahu.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gynnsfpez.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/geywakwce.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcodpdxrb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gngfymuss.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gzqoosaim.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyjnqdvw.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gudxfytgy.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzfviatxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ghovsynak.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gzrbsjmke.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gedflxcgr.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvwpycgy.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gkgdvunqo.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyijlnuj.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/grkxjrfxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncyqxtcq.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwfbxrnd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gedaatbqj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmdrvjk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gagwkmgux.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gsuuwgrcv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gidkmhpsx.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gjuntifen.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdzdurqj.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gnjycyuls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gozjhfnds.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gssclttim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqsmhcnl.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gimbpxjof.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifvczvcq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gsceccuda.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkyrxset.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzyvhnvsy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/galmeylqd.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqzfbzici.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/glfhhygqh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gebslusdq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydqbkncz.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkqljewa.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuiqvmkt.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ghrazsffe.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteuwkuuu.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gofduxcmv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxdachvyz.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiqsoutx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvdwwref.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyeaqvsv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gotaowvdn.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbuuwgavv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gafvbfqqv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixauslsm.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsgjqewzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gluuyzwfs.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gezmeucpc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmerjkqjf.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkfczhutg.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gedyfznpj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/grkxfvcsg.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvnugyns.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammdlriy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukztukd.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gshncyhoo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqfgtwvx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckxflen.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsviykvnq.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gnonvniih.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjcftis.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuamjzav.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gapucdrcd.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzvizvkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/geyxtzcje.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gcjhghjbc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztskcyl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojepebec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrlqxkze.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzexpmkzw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvtuxdh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxkncdd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gymoacbsv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrsqmcni.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbysgptr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmhaumzj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygbgsyu.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggokfavkf.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gvjanomzi.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkqgudvxq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gbxpkkcji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwofxkzpx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gevfvlfce.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjyabjhjs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gkwlnbyew.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmayrmvzh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmxhgtf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gropqtyua.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyindgeg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsmsdhza.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqkbyqjl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcouowpev.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/giwixuvxo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcktcyuyz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqjgcsz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwixcqvse.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gojmrunai.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjcmtecg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqvcnama.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gxyjemads.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/griblrmlm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyipfdlhz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkorkzqmy.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geqapdheg.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/glwvyurtg.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpgbriniy.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrwawxhs.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gggvukfeu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaohpddxy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/genzkuomz.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaqeicgp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesinkbiz.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gthugaggx.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimeiidcm.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/giwsmldrj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvmilfebf.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfzuizolt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/geeylhjrc.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdegbwhmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpowxwpff.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gveizydph.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/geuawlnxl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuitgnsz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgiagnfc.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gotpymhsv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxdbrbapr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlimvolb.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykbpoxtl.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrcrxbzc.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gmpsinoif.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcluiwxfn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmaroqf.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqaxunhxa.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnaqgaet.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyobzbsuj.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqphlxtuf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxckawvw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gazffscnf.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gbuusfyul.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gnumlamdz.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gaygcbwgl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gakyceedu.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glhtndchz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqxdhlxe.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzdwwcfs.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyxmcrhd.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxljfmdq.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gphcqpzfg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvareqskm.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/geopotadc.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gtngkwplg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/giytuqnbt.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/guermstjj.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpxoiedk.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmjngkxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzivrpkxu.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwwboys.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaraetim.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqezmqeyo.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxiscjb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchtgdtjr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gazcuqkrk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpomijgso.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshueuiz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsfzqyfj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gofaifsgd.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gngdqzfhf.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gviqvqbwi.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyylkjalr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gacxaqifd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrlunyx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicyxdzsp.sHtML


<!-- 参考信息 -->