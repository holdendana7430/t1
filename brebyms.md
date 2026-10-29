代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gcxgtqgpq.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gpbievzoc.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gyzmhwmzl.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/ggkhppbjw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gbrucesyg.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gdetfguzq.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvvuutbqx.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gtdkvtfxp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/grvzeuiau.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gmdxollqu.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gsrihsozm.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gdzgtocyu.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/glzerovzr.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gjmofmdtx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/griqayyol.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gfoetrvfa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gsnmmuldk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gpsowyxyq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gpzuinyqm.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gajhilkmi.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gmjotmcbl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gcwlyinyd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/geuhewxxj.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gihzsfvuh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gjhxfwlhp.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gmdfcmocn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gomucszqf.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gpbhzfean.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gifzssxbj.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gzhvvphbr.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gymslueec.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gxpeofccx.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gzbxswgaw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gmcedbnau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gudhxevjo.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gtqfootwi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gnqnbfbdd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gwnmxgkju.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gtcjmurow.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqoerlwzb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gacqtkrcz.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gjojjpjmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gkycrlyki.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/ggstlghqi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gkwhgurvr.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/growcndmu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gejykqlex.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gpgvjigmi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gaiampcdf.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gxfntrqzb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grywybtwe.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gnbfozvrl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gfcyghykw.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gbelgligl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glzlkwrsd.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gsclfnntb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gjgdfsuxm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/grfovsahs.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gnxfiuimx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvvwztbkd.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gftspqjcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmequylju.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwsaylwur.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ghzbgytut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gsysaehsx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gavyvrwcw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gjomalkgh.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gbihixcot.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gynxlgnpj.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gaxznmaep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gaemujtlk.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gkbsoxcgr.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gnymfhvsw.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/glbaexylb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gbbqtcsxv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gwzdblmwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzrywvurk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gykmpknnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gvmxiddgr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gocxjtsbf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gruztpdhb.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gjddnpeqh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gmeoituxx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcvgyhbly.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gyopnwlyf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gccxjohay.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gjhbmccpi.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gdnbfnbur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvsztcdvt.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/glozjbaen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfkevjhij.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gqioakoci.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gvkvypcgz.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfudpbpnl.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/guiyradev.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gxkfjhiln.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gvaafydsg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwxkmdkzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gtejalqrm.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gxehdxmnw.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gwsmoumwq.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gtpscejvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gpujobtlk.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gqwlhfyrs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxcjxgfal.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gmalqdohq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gmrgcyfwy.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gsamfiisj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gptuebwjv.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gkmmsgzii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gxrihssmi.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ghvqduyze.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gqsmvwnrk.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gngfchhpj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gzxbesjml.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gwfhdnkjs.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gflxngcoy.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gnqurdten.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkcbxxwsi.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gfifaqnsh.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gsidbxfol.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gfphnuxnu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gtpypesfa.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gjzaabzok.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gxdtyznjk.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ghrlhgbti.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/ggwqxdtri.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvsncsqlk.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gpadxcdwi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gpcbyveuw.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gveamlnvf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gkqdyxnsx.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gaynpiesf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnrzrqxsw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/glcscrnai.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gqgajqnqy.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/ggaccemrr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/graqpjqaw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gbbmfbpbi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkxzwvslw.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/glpowvakc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/govqknbhr.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gjtubiffz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gniscjnxk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gyelnydmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gnsnzmjmd.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gemvsnwik.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gdzpygpbt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtkxoygxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gdyyowtwb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpvizdfwe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gxltadaql.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gwruwkghs.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gtkoeldqr.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/geamzjxnw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwepdbmmx.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gzexjvkbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gyhlhiral.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/glzcjqjgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ghzjpjbib.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gchgtxjfg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/ggtrltrdh.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfikvsenv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gvphhefxh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxltlse.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gswtynejx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gajnmclrw.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gbyifwcki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gomrstrkx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/grdedmgme.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gqzgvzlxr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gchekehtw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/grhloljqs.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gjvtgnyni.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gpjyyuwea.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gjaokebeg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/golzkwxgi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gxodiyqgl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxbzcplbv.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gfokmvyvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/guwlrjrhb.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gvsvclibc.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxfbvcicv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gbvipguxs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtelhnakq.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gdjxmgepb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gbwjoxytg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gynzvpbwi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gkqkqurkv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsnwtxuak.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/geboebjqb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmluovrjf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glslalvzh.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/grfzwgrvk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gplqowsdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gwlbirtam.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gwxdellbi.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gghpmndrz.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gpquiztqg.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gkguytepx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gwiintumx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gnjjztmrh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvhvgpbmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gzbpxannv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gahopmoop.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gmajtiibp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gprklezpo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gnpfbmdio.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gkdnqmkrg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqahebixy.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gthzjsfcb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gotwwybwu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/grvuuteys.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/griilmugi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/ghwpomzlg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbrfxdvbv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gkcygwunp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwizwklhd.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gyjazgeoh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gazsxsrqe.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gphhsqdmv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gdxfkpyvg.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gntlehoaz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grsfpqndn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gykxybzfj.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gqmfcgkij.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gaayohgjk.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gqkkjjsli.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/giuvffmxm.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gegffcmtm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gzncefdmn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gtgzfhfkn.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gxjtehfrc.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gpciuiuaj.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/giyxwsmjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gloxnopww.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gjnfsmopp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gtpgiwier.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gqfbmkgyx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghawyjlxw.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/glqfffyqd.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gcejqmeil.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gekszzqbi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gahfyniyr.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gbphkcvka.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gndqqdcls.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gushaeoqe.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gzfgbelnw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gifypulxf.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/guudyjtuc.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gyfzxweaf.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gdrxpyfof.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gvwzbkird.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpkubfmow.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/giubexpsn.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gpjgparpm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gtvvfgkww.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gzlxhxenf.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gluttvame.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/grszdmbvk.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gpuuvmprz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxnrsjfgd.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gkxyeqpgy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glcaexotn.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gedrymsxw.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gkxxfvfds.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gkysvrhth.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gncutrzuz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/grqxbupic.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gwxzfciah.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gmlyeizbb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/ghcirfyun.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghfglkuos.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gpmioierq.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gavnsmfwd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gmrsgkqcz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gzxwoobdh.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gdpbcldsa.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gqaujyouy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gmemdwukg.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/guqofrqrg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gkvnerkyc.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gpxzgxwky.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/giywjpbnb.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gbzxpwjiq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcoltbvwz.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gjzzwefsv.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gnwokgvrw.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gydvmbkrq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdovhiyn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcmemmuqc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gghqsklme.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gpejsoqof.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkcgawpdw.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxiwqsupc.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/ggsolxlwl.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gfmskvccq.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/ggfstmpxm.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gqncqcnhq.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gncvskaza.sHtML


<!-- 参考信息 -->